# b00b0-sparkrun

Recipe registry for [sparkrun](https://github.com/spark-arena/sparkrun) with llama-benchy benchmark results on a single DGX GX10 node.

## Repository Structure

```
recipe-registry/          # vLLM serving recipes (.yaml)
  .sparkrun/
    registry.yaml         # sparkrun registry declaration
assets/
  llama-benchy-results/   # benchmark output files (.md), one per recipe
```

Recipes follow the naming convention `<hf-org>_<model-slug>.<quant>.yaml`.  
Benchmark result files share the same name with a `.md` extension.  
Files prefixed with `@` are experimental results without a corresponding stable recipe.

## Benchmark Results

All results on a single DGX GX10 · `pp=2048, tg=32` · averages across runs.

| Recipe | Results | pp2048 c=1 | tg32 c=1 | pp2048 c=4 | tg32 c=4 |
|--------|---------|:----------:|:--------:|:----------:|:--------:|
| [crushleorey_qwopus3.6-27b-nvfp4.yaml](recipe-registry/crushleorey_qwopus3.6-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/crushleorey_qwopus3.6-27b-nvfp4.md) | 1886.7 | 21.0 | 2504.1 | 63.1 |
| [google_gemma-4-26b-a4b-fp8.yaml](recipe-registry/google_gemma-4-26b-a4b-fp8.yaml) | [📊](assets/llama-benchy-results/google_gemma-4-26b-a4b-fp8.md) | 5992.5 | 40.1 | 6753.1 | 77.3 |
| [jackrong_qwopus3.6-27b-coder-fp8.yaml](recipe-registry/jackrong_qwopus3.6-27b-coder-fp8.yaml) | [📊](assets/llama-benchy-results/jackrong_qwopus3.6-27b-coder-fp8.md) | — | — | 512.2 | 54.1 |
| [jackrong_qwopus3.6-27b-v2-fp8.yaml](recipe-registry/jackrong_qwopus3.6-27b-v2-fp8.yaml) | [📊](assets/llama-benchy-results/jackrong_qwopus3.6-27b-v2-fp8.md) | 589.5 | 16.3 | 590.1 | 53.9 |
| [nvidia_gemma-4-26b-a4b-nvfp4.yaml](recipe-registry/nvidia_gemma-4-26b-a4b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_gemma-4-26b-a4b-nvfp4.md) | 5994.6 | 30.0 | 6466.5 | 71.2 |
| [nvidia_gemma-4-31b-nvfp4.yaml](recipe-registry/nvidia_gemma-4-31b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_gemma-4-31b-nvfp4.md) | 1790.0 | 6.8 | 1788.8 | 19.3 |
| [nvidia_qwen3.6-35b-a3b-nvfp4.yaml](recipe-registry/nvidia_qwen3.6-35b-a3b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_qwen3.6-35b-a3b-nvfp4.md) | 2823.2 | 108.1 | 5605.2 | 257.5 |
| [prismascout_qwen3.6-27b-nvfp4.yaml](recipe-registry/prismascout_qwen3.6-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/prismascout_qwen3.6-27b-nvfp4.md) | 1942.1 | 25.9 | 2362.8 | 92.8 |
| [redhatai_qwen3.6-35b-a3b-dflash-nvfp4.yaml](recipe-registry/redhatai_qwen3.6-35b-a3b-dflash-nvfp4.yaml) | [📊](assets/llama-benchy-results/redhatai_qwen3.6-35b-a3b-dflash-nvfp4.md) | 5197.7 | 119.3 | 6127.9 | 165.8 |
| [unsloth_qwen3.6-27b-nvfp4.yaml](recipe-registry/unsloth_qwen3.6-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/unsloth_qwen3.6-27b-nvfp4.md) | 1873.8 | 21.6 | 1916.5 | 74.5 |
| [unsloth_qwen3.6-35b-a3b-nvfp4.yaml](recipe-registry/unsloth_qwen3.6-35b-a3b-nvfp4.yaml) | — | — | — | — | — |

### Experimental

Results without a stable recipe (prefix `@`):

| Results | Notes |
|---------|-------|
| [📊 v1](assets/llama-benchy-results/@experimental_qwen3.6-27b-fp8-dflash-512k-vllm_v1.md) | Qwen3.6-27B FP8 DFlash 512k context — run 1 |
| [📊 v2](assets/llama-benchy-results/@experimental_qwen3.6-27b-fp8-dflash-512k-vllm_v2.md) | Qwen3.6-27B FP8 DFlash 512k context — run 2 |

## Acknowledgements

- [llama-benchy](https://github.com/eugr/llama-benchy) — benchmarking tool used to generate all results
- [spark-vllm-docker](https://github.com/eugr/spark-vllm-docker) — Docker images powering the vLLM containers
- [sparkrun](https://github.com/spark-arena/sparkrun) — recipe runner this registry is built for
