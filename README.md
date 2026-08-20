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
| [nvidia_qwen3.6-35b-a3b-nvfp4.yaml](recipe-registry/nvidia_qwen3.6-35b-a3b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_qwen3.6-35b-a3b-nvfp4.md) | 4866.0 | 106.7 | 6210.3 | 251.7 |
| [qwen3.6-35b-a3b-autoround-int4-dflash-vllm-cipherfoxie.yaml](https://github.com/spark-arena/community-recipe-registry/blob/main/recipes/qwen3.6-35b-a3b/cipherfoxie/qwen3.6-35b-a3b-autoround-int4-dflash-vllm-cipherfoxie.yaml) | [📊](assets/llama-benchy-results/@community_qwen3.6-35b-a3b-autoround-int4-dflash-vllm-cipherfoxie.md) | 4790.0 | 69.9 | 5867.2 | 138.1 |
| [qwen3.6-27b-fp8-dflash-512k-vllm.yaml](https://github.com/spark-arena/recipe-registry/blob/main/experimental-recipes/qwen3.6/vllm-dflash/qwen3.6-27b-fp8-dflash-512k-vllm.yaml) | [📊](assets/llama-benchy-results/@experimental_qwen3.6-27b-fp8-dflash-512k-vllm_v1.md) | 1396.1 | 26.9 | 708.6 | 86.7 |
| [deepreinforce-ai_ornith-1.0-35b-fp8-nomtp.yaml](recipe-registry/deepreinforce-ai_ornith-1.0-35b-fp8-nomtp.yaml) | [📊](assets/llama-benchy-results/deepreinforce-ai_ornith-1.0-35b-fp8-nomtp.md) | 4936.5 | 39.6 | 5928.9 | 80.2 |
| [jackrong_qwopus3.6-35b-a3b-coder-fp8.yaml](recipe-registry/jackrong_qwopus3.6-35b-a3b-coder-fp8.yaml) | [📊](assets/llama-benchy-results/jackrong_qwopus3.6-35b-a3b-coder-fp8.md) | 3987.7 | 51.5 | 4673.7 | 73.2 |
| [qwen3.6-27b-fp8-dflash-vllm.yaml](https://github.com/spark-arena/recipe-registry/blob/main/experimental-recipes/qwen3.6/vllm-dflash/qwen3.6-27b-fp8-dflash-vllm.yaml) | [📊](assets/llama-benchy-results/@experimental_qwen3.6-27b-fp8-dflash-vllm.md) | 1486.5 | 31.8 | 880.5 | 69.7 |
| [nvidia_qwen3.6-27b-nvfp4.yaml](recipe-registry/nvidia_qwen3.6-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/nvidia_qwen3.6-27b-nvfp4.md) | 1043.5 | 46.9 | 1080.6 | 57.1 |
| [jackrong_qwopus3.6-27b-coder-fp8.yaml](recipe-registry/jackrong_qwopus3.6-27b-coder-fp8.yaml) | [📊](assets/llama-benchy-results/jackrong_qwopus3.6-27b-coder-fp8.md) | 643.3 | 17.6 | 533.2 | 53.3 |
| [radixark_qwen3.8-27b-nvfp4.yaml](recipe-registry/radixark_qwen3.8-27b-nvfp4.yaml) | [📊](assets/llama-benchy-results/radixark_qwen3.8-27b-nvfp4.md) | 1612.6 | 17.9 | 2040.5 | 49.9 |
| [empero-ai_qwythos-9b-mythos.yaml](recipe-registry/empero-ai_qwythos-9b-mythos.yaml) | [📊](assets/llama-benchy-results/empero-ai_qwythos-9b-mythos.md) | 3366.8 | 23.8 | 3519.5 | 49.4 |
| [redhatai_muse-glimmer-30b-fp8-block.yaml](recipe-registry/redhatai_muse-glimmer-30b-fp8-block.yaml) | [📊](assets/llama-benchy-results/redhatai_muse-glimmer-30b-fp8-block.md) | 1717.1 | 16.2 | 2049.9 | 42.8 |

## Acknowledgements

- [llama-benchy](https://github.com/eugr/llama-benchy) — benchmarking tool used to generate all results
- [spark-vllm-docker](https://github.com/eugr/spark-vllm-docker) — Docker images powering the vLLM containers
- [sparkrun](https://github.com/spark-arena/sparkrun) — recipe runner this registry is built for
