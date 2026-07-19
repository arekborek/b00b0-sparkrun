(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:27:04
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-35b-a3b': nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cc298-57fc3fba6e40cda142e0843b;75c3cb70-11eb-4449-94a6-5f15ad680652)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-35b-a3b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 2.73 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |             t/s |      peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|----------------:|--------------:|--------------:|---------------:|----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 | 4897.09 ± 34.90 |               | 400.86 ± 8.18 |  398.13 ± 8.18 |   400.86 ± 8.18 |
| nvidia/qwen3.6-35b-a3b |   tg32 |   113.41 ± 7.09 | 117.07 ± 7.32 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:27:04 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:27:14
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-35b-a3b': nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cc2a2-31e9c55a33ea66233fbb2dec;ec382fdf-d59e-4be4-af22-ca1a8be1a2d3)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-35b-a3b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 5.09 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |             t/s |      peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|----------------:|--------------:|--------------:|---------------:|----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 | 4868.36 ± 59.69 |               | 385.96 ± 7.74 |  380.87 ± 7.74 |   385.96 ± 7.74 |
| nvidia/qwen3.6-35b-a3b |   tg32 |   105.50 ± 0.33 | 108.90 ± 0.34 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:27:14 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:27:22
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-35b-a3b': nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cc2aa-1b606e771f834b986936155a;373e5248-bc1f-41bf-ab2b-b8c742d0c0aa)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-35b-a3b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.13 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |             t/s |      peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|----------------:|--------------:|--------------:|---------------:|----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 | 4832.64 ± 59.56 |               | 389.04 ± 6.22 |  385.91 ± 6.22 |   389.04 ± 6.22 |
| nvidia/qwen3.6-35b-a3b |   tg32 |   101.25 ± 5.51 | 104.52 ± 5.69 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:27:22 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:27:30
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-35b-a3b': nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cc2b3-45f77ed830cd69561cd8f810;acf974e9-ffe5-43d5-abe0-91d76254a983)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-35b-a3b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.06 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |     t/s (total) |       t/s (req) |       peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|------------:|----------------:|----------------:|---------------:|-----------------:|----------------:|----------------:|----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 (c4) | 6271.23 ± 99.00 | 1591.93 ± 51.73 |                |                  | 1183.66 ± 34.71 | 1179.60 ± 34.71 | 1183.66 ± 34.71 |
| nvidia/qwen3.6-35b-a3b |   tg32 (c4) |  241.45 ± 51.33 |   77.22 ± 10.61 | 249.24 ± 52.98 |    79.71 ± 10.95 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:27:30 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:27:47
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-35b-a3b': nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cc2c3-6fbe3d2e1884bf107e3d0cc5;e8cedaa2-6dae-4b6c-a07d-882f33b0c414)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-35b-a3b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.53 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |     t/s (total) |       t/s (req) |       peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|------------:|----------------:|----------------:|---------------:|-----------------:|----------------:|----------------:|----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 (c4) | 6136.00 ± 44.41 | 1558.04 ± 76.93 |                |                  | 1196.58 ± 26.66 | 1193.06 ± 26.66 | 1196.58 ± 26.66 |
| nvidia/qwen3.6-35b-a3b |   tg32 (c4) |  246.26 ± 20.05 |    76.28 ± 8.82 | 254.20 ± 20.69 |     78.74 ± 9.11 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:27:47 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:28:02
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-35b-a3b': nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cc2d2-42933d652de962c371e989b4;7af47ab1-3423-4f9b-9cc2-273a23875dce)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-35b-a3b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.98 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |      t/s (total) |       t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|------------:|-----------------:|----------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 (c4) | 6223.64 ± 125.12 | 1581.72 ± 78.02 |               |                  | 1180.56 ± 25.54 | 1176.57 ± 25.54 | 1180.56 ± 25.54 |
| nvidia/qwen3.6-35b-a3b |   tg32 (c4) |    267.36 ± 5.87 |    78.94 ± 5.22 | 275.98 ± 6.06 |     81.49 ± 5.39 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:28:02 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
