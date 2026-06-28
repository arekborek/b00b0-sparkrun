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

## Usage

### Add this registry

```bash
sparkrun registry add "https://github.com/arekborek/b00b0-sparkrun/recipe-registry"
```

### Run and stop a recipe

Recipes run in the background — you can close the terminal after launch.

```bash
sparkrun -v run @arek/jackrong_qwopus3.6-27b-coder-fp8
sparkrun stop  @arek/jackrong_qwopus3.6-27b-coder-fp8

sparkrun -v run  @experimental/qwen3.6-27b-fp8-dflash-512k-vllm
sparkrun stop    @experimental/qwen3.6-27b-fp8-dflash-512k-vllm
```

### Proxy

Run a single endpoint in front of all served models (backed by LiteLLM):

```bash
sparkrun proxy start
sparkrun proxy stop
sparkrun proxy models
sparkrun proxy status
```

### Search

```bash
sparkrun list -a | grep -E "qwen3.6.*(fp8|nvfp4)"
```

## Benchmark Results

All results on a single DGX GX10 · `pp=2048, tg=32` · averages across runs.

| Recipe | Results | pp2048 c=1 | tg32 c=1 | pp2048 c=4 | tg32 c=4 |
|--------|---------|:----------:|:--------:|:----------:|:--------:|
| [nvidia_qwen3.6-35b-a3b-nvfp4.yaml](recipe-registry/nvidia_qwen3.6-35b-a3b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_qwen3.6-35b-a3b-nvfp4.md) | 2823.2 | 108.1 | 5605.2 | 257.5 |
| [redhatai_qwen3.6-35b-a3b-dflash-nvfp4.yaml](recipe-registry/redhatai_qwen3.6-35b-a3b-dflash-nvfp4.yaml) | [📊](assets/llama-benchy-results/redhatai_qwen3.6-35b-a3b-dflash-nvfp4.md) | 5197.7 | 119.3 | 6127.9 | 165.8 |
| [prismascout_qwen3.6-27b-nvfp4.yaml](recipe-registry/prismascout_qwen3.6-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/prismascout_qwen3.6-27b-nvfp4.md) | 1942.1 | 25.9 | 2362.8 | 92.8 |
| [qwen3.6-27b-fp8-dflash-512k-vllm.yaml](https://github.com/spark-arena/recipe-registry/blob/main/experimental-recipes/qwen3.6/vllm-dflash/qwen3.6-27b-fp8-dflash-512k-vllm.yaml) | [📊](assets/llama-benchy-results/@experimental_qwen3.6-27b-fp8-dflash-512k-vllm_v1.md) | 1396.1 | 26.9 | 708.6 | 86.7 |
| [google_gemma-4-26b-a4b-fp8.yaml](recipe-registry/google_gemma-4-26b-a4b-fp8.yaml) | [📊](assets/llama-benchy-results/google_gemma-4-26b-a4b-fp8.md) | 5992.5 | 40.1 | 6753.1 | 77.3 |
| [unsloth_qwen3.6-27b-nvfp4.yaml](recipe-registry/unsloth_qwen3.6-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/unsloth_qwen3.6-27b-nvfp4.md) | 1873.8 | 21.6 | 1916.5 | 74.5 |
| [nvidia_gemma-4-26b-a4b-nvfp4.yaml](recipe-registry/nvidia_gemma-4-26b-a4b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_gemma-4-26b-a4b-nvfp4.md) | 5994.6 | 30.0 | 6466.5 | 71.2 |
| [crushleorey_qwopus3.6-27b-nvfp4.yaml](recipe-registry/crushleorey_qwopus3.6-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/crushleorey_qwopus3.6-27b-nvfp4.md) | 1886.7 | 21.0 | 2504.1 | 63.1 |
| [jackrong_qwopus3.6-27b-coder-fp8.yaml](recipe-registry/jackrong_qwopus3.6-27b-coder-fp8.yaml) | [📊](assets/llama-benchy-results/jackrong_qwopus3.6-27b-coder-fp8.md) | — | — | 512.2 | 54.1 |
| [jackrong_qwopus3.6-27b-v2-fp8.yaml](recipe-registry/jackrong_qwopus3.6-27b-v2-fp8.yaml) | [📊](assets/llama-benchy-results/jackrong_qwopus3.6-27b-v2-fp8.md) | 589.5 | 16.3 | 590.1 | 53.9 |
| [nvidia_gemma-4-31b-nvfp4.yaml](recipe-registry/nvidia_gemma-4-31b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_gemma-4-31b-nvfp4.md) | 1790.0 | 6.8 | 1788.8 | 19.3 |
| [unsloth_qwen3.6-35b-a3b-nvfp4.yaml](recipe-registry/unsloth_qwen3.6-35b-a3b-nvfp4.yaml) | — | — | — | — | — |

## Acknowledgements

- [llama-benchy](https://github.com/eugr/llama-benchy) — benchmarking tool used to generate all results
- [spark-vllm-docker](https://github.com/eugr/spark-vllm-docker) — Docker images powering the vLLM containers
- [sparkrun](https://github.com/spark-arena/sparkrun) — recipe runner this registry is built for
