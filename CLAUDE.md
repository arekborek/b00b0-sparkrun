# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

A registry of vLLM serving recipes for NVIDIA DGX/Blackwell hardware, paired with benchmark results. There is no build system, test suite, or application code — this is a declarative data repository.

## Launching a recipe

```bash
sparkrun recipe-registry/<recipe-name>.yaml
```

Override any default at launch time:

```bash
sparkrun recipe-registry/nvidia_qwen3.6-35b-a3b-nvfp4.yaml \
  --tensor-parallel 2 \
  --max-model-len 131072
```

## Running a benchmark

Run at two concurrency levels and save both outputs to a single file:

```bash
llama-benchy \
  --base-url "http://<host>:<port>/v1" \
  --model "<served-model-name>" \
  --concurrency 1

llama-benchy \
  --base-url "http://<host>:<port>/v1" \
  --model "<served-model-name>" \
  --concurrency 4
```

Save terminal output to `assets/llama-benchy-results/<recipe-name>.md` (filename must match the recipe file, without the `.yaml` extension).

## Recipe YAML schema

Key fields and their role:

| Field | Notes |
|-------|-------|
| `recipe_version` | Always `"1"` |
| `model` | HuggingFace model ID used by `--download-model` |
| `container` | Docker image from `ghcr.io/spark-arena/` — use `dgx-vllm-eugr-nightly-tf5` for TF5 / DFlash builds |
| `mods` | Ordered list of patch names applied before launch |
| `defaults` | Overridable vLLM flags; referenced in `command` as `{key}` placeholders |
| `env` | Environment variables injected into the container |
| `command` | Shell template for `vllm serve`; uses `{placeholder}` syntax for `defaults` values |
| `cluster_only` / `solo_only` | Deployment constraints; omit or set `false` for general use |

## Naming conventions

Recipe files: `<hf-org>_<model-slug>.<quant>.yaml`, e.g. `nvidia_qwen3.6-35b-a3b-nvfp4.yaml`.

Benchmark result files: identical name, `.md` extension, in `assets/llama-benchy-results/`.

Prefix experimental/unstable results with `@` (e.g. `@experimental_qwen3.6-27b-fp8-dflash-512k-vllm.md`) when no corresponding stable recipe exists.

## Architecture decisions in recipes

- **NVFP4 models**: use `load_format: instanttensor`, `kv_cache_dtype: fp8`, `attention_backend: flashinfer`, and `VLLM_MARLIN_USE_ATOMIC_ADD: "1"`.
- **DFlash speculative decoding**: set `--speculative-config '{"method":"dflash","model":"<draft-model>","num_speculative_tokens":<n>}'`; use the `dgx-vllm-eugr-nightly-tf5` container image.
- **MTP speculative decoding**: set `--speculative-config '{"method":"mtp","num_speculative_tokens":<n>}'` (supported in the standard nightly image).
- **FP8 online quantization**: omit `load_format`, pass `--quantization fp8` in the command instead.
- **Qwen3.x models** consistently need `mods/fix-qwen3-coder-next` and often `mods/fix-qwen3.5-chat-template`.

## Updating README.md

When adding a new recipe with benchmark results, add a row to the table in `README.md` linking the recipe filename and reporting averaged `pp2048 t/s` and `tg32 t/s` at `c=1` and `c=4`. Leave cells empty if benchmarks haven't been collected yet.

## Git & Branching

- **Model:** GitHub Flow — feature branches off `main`, merged via PR.
- **Default branch:** `main`
- **Branch naming:** `<type>/<short-description>` — e.g. `feature/add-login`, `fix/null-pointer`
- **Commit convention:** Conventional Commits — `<type>(<scope>): <summary>` (e.g. `feat(auth): add OAuth2 login`)
- **Landing changes:** PR required; at least one approval before merge; author merges after approval.
- **Merge strategy:** Squash merge — one commit per PR on the default branch.
- **Claude's permissions:** Prepare changes only — Claude commits locally but does **not** push or open PRs unless explicitly asked.
- **Protected branches / rules:** `main` is protected — no direct pushes; all changes via PR.
