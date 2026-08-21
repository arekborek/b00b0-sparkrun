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

All results on a single DGX GX10 · `pp=2048, tg=32` · average of per-run upper bounds (`mean + stdev`).

| Recipe | Results | pp2048 c=1 | tg32 c=1 | pp2048 c=4 | tg32 c=4 |
|--------|---------|:----------:|:--------:|:----------:|:--------:|
| [nvidia_qwen3.6-35b-a3b-nvfp4.yaml](recipe-registry/nvidia_qwen3.6-35b-a3b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_qwen3.6-35b-a3b-nvfp4.md) | 4917.4 | 111.0 | 6299.8 | 277.4 |
| [qwen3.6-35b-a3b-autoround-int4-dflash-vllm-cipherfoxie.yaml](https://github.com/spark-arena/community-recipe-registry/blob/main/recipes/qwen3.6-35b-a3b/cipherfoxie/qwen3.6-35b-a3b-autoround-int4-dflash-vllm-cipherfoxie.yaml) | [📊](assets/llama-benchy-results/@community_qwen3.6-35b-a3b-autoround-int4-dflash-vllm-cipherfoxie.md) | 4921.7 | 80.6 | 5896.4 | 142.4 |
| [qwen3.6-27b-fp8-dflash-512k-vllm.yaml](https://github.com/spark-arena/recipe-registry/blob/main/experimental-recipes/qwen3.6/vllm-dflash/qwen3.6-27b-fp8-dflash-512k-vllm.yaml) | [📊](assets/llama-benchy-results/@experimental_qwen3.6-27b-fp8-dflash-512k-vllm_v1.md) | 1499.9 | 28.7 | 857.1 | 100.2 |
| [qwen3.6-27b-fp8-dflash-512k-vllm.yaml](https://github.com/spark-arena/recipe-registry/blob/main/experimental-recipes/qwen3.6/vllm-dflash/qwen3.6-27b-fp8-dflash-512k-vllm.yaml) | [📊](assets/llama-benchy-results/@experimental_qwen3.6-27b-fp8-dflash-512k-vllm_v2.md) |  |  | 1125.8 | 89.3 |
| [qwen3.6-27b-fp8-dflash-vllm.yaml](https://github.com/spark-arena/recipe-registry/blob/main/experimental-recipes/qwen3.6/vllm-dflash/qwen3.6-27b-fp8-dflash-vllm.yaml) | [📊](assets/llama-benchy-results/@experimental_qwen3.6-27b-fp8-dflash-vllm.md) | 1538.0 | 35.2 | 1071.6 | 88.3 |
| [deepreinforce-ai_ornith-1.0-35b-fp8-nomtp.yaml](recipe-registry/deepreinforce-ai_ornith-1.0-35b-fp8-nomtp.yaml) | [📊](assets/llama-benchy-results/deepreinforce-ai_ornith-1.0-35b-fp8-nomtp.md) | 4972.6 | 39.7 | 5943.9 | 81.8 |
| [jackrong_qwopus3.6-35b-a3b-coder-fp8.yaml](recipe-registry/jackrong_qwopus3.6-35b-a3b-coder-fp8.yaml) | [📊](assets/llama-benchy-results/jackrong_qwopus3.6-35b-a3b-coder-fp8.md) | 4260.6 | 51.8 | 5331.5 | 76.8 |
| [nvidia_qwen3.6-27b-nvfp4.yaml](recipe-registry/nvidia_qwen3.6-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_qwen3.6-27b-nvfp4.md) | 1046.0 | 51.3 | 1082.8 | 60.6 |
| [jackrong_qwopus3.6-27b-coder-fp8.yaml](recipe-registry/jackrong_qwopus3.6-27b-coder-fp8.yaml) | [📊](assets/llama-benchy-results/jackrong_qwopus3.6-27b-coder-fp8.md) | 644.8 | 19.0 | 594.5 | 57.1 |
| [radixark_qwen3.8-27b-nvfp4.yaml](recipe-registry/radixark_qwen3.8-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/radixark_qwen3.8-27b-nvfp4.md) | 1831.7 | 19.3 | 2117.4 | 52.0 |
| [empero-ai_qwythos-9b-mythos.yaml](recipe-registry/empero-ai_qwythos-9b-mythos.yaml) | [📊](assets/llama-benchy-results/empero-ai_qwythos-9b-mythos.md) | 3377.9 | 23.8 | 3526.4 | 49.8 |
| [redhatai_muse-glimmer-30b-fp8-block.yaml](recipe-registry/redhatai_muse-glimmer-30b-fp8-block.yaml) | [📊](assets/llama-benchy-results/redhatai_muse-glimmer-30b-fp8-block.md) | 1766.0 | 20.8 | 2078.8 | 44.2 |

## Acknowledgements

- [llama-benchy](https://github.com/eugr/llama-benchy) — benchmarking tool used to generate all results
- [spark-vllm-docker](https://github.com/eugr/spark-vllm-docker) — Docker images powering the vLLM containers
- [sparkrun](https://github.com/spark-arena/sparkrun) — recipe runner this registry is built for
