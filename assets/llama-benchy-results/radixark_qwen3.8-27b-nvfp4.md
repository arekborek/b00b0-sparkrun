(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "radixark/qwen3.8-27b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 16:21:26
Benchmarking model: radixark/qwen3.8-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'radixark/qwen3.8-27b': radixark/qwen3.8-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a870d66-0b973daa1286d5a024e99ca7;ecf2fc79-fb69-43b4-94df-e1e89e2b8752)

Repository Not Found for url: https://huggingface.co/radixark/qwen3.8-27b/resolve/main/tokenizer.json.
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
Average latency (api): 3.55 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                |   test |             t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:---------------------|-------:|----------------:|-------------:|---------------:|---------------:|----------------:|
| radixark/qwen3.8-27b | pp2048 | 1461.15 ± 15.70 |              | 1266.66 ± 4.80 | 1263.11 ± 4.80 |  1266.66 ± 4.80 |
| radixark/qwen3.8-27b |   tg32 |    17.56 ± 2.45 | 19.67 ± 3.09 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 16:21:26 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "radixark/qwen3.8-27b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 16:21:58
Benchmarking model: radixark/qwen3.8-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'radixark/qwen3.8-27b': radixark/qwen3.8-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a870d87-3cd2936b5171e5cd6ab85e6a;1c3f6674-f99c-4e17-b3be-877915199187)

Repository Not Found for url: https://huggingface.co/radixark/qwen3.8-27b/resolve/main/tokenizer.json.
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
Average latency (api): 3.27 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                |   test |              t/s |     peak t/s |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:---------------------|-------:|-----------------:|-------------:|-----------------:|-----------------:|-----------------:|
| radixark/qwen3.8-27b | pp2048 | 1693.44 ± 330.64 |              | 1152.73 ± 163.96 | 1149.46 ± 163.96 | 1152.73 ± 163.96 |
| radixark/qwen3.8-27b |   tg32 |     18.70 ± 0.56 | 21.33 ± 1.25 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 16:21:58 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "radixark/qwen3.8-27b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 16:22:16
Benchmarking model: radixark/qwen3.8-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'radixark/qwen3.8-27b': radixark/qwen3.8-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a870d99-16ad271e61305f5b3c5cd8c2;2d7bd7fb-ba8d-4b39-a833-7357ab5fd5e0)

Repository Not Found for url: https://huggingface.co/radixark/qwen3.8-27b/resolve/main/tokenizer.json.
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
Average latency (api): 2.98 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                |   test |              t/s |     peak t/s |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:---------------------|-------:|-----------------:|-------------:|-----------------:|-----------------:|-----------------:|
| radixark/qwen3.8-27b | pp2048 | 1683.28 ± 310.86 |              | 1121.06 ± 220.04 | 1118.08 ± 220.04 | 1121.06 ± 220.04 |
| radixark/qwen3.8-27b |   tg32 |     17.58 ± 0.95 | 19.33 ± 0.47 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 16:22:16 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "radixark/qwen3.8-27b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 16:23:03
Benchmarking model: radixark/qwen3.8-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'radixark/qwen3.8-27b': radixark/qwen3.8-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a870dc8-4f3e484b0955113a0a41f1b8;7fd015b1-c372-420e-bb4c-03df00a097a2)

Repository Not Found for url: https://huggingface.co/radixark/qwen3.8-27b/resolve/main/tokenizer.json.
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
Average latency (api): 3.84 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |      t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:---------------------|------------:|-----------------:|---------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| radixark/qwen3.8-27b | pp2048 (c4) | 2099.64 ± 133.10 | 531.01 ± 39.99 |              |                  | 3494.68 ± 289.81 | 3490.84 ± 289.81 | 3494.68 ± 289.81 |
| radixark/qwen3.8-27b |   tg32 (c4) |     52.07 ± 1.36 |   14.64 ± 1.33 | 64.33 ± 3.09 |     17.75 ± 2.05 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 16:23:03 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "radixark/qwen3.8-27b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 16:23:35
Benchmarking model: radixark/qwen3.8-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'radixark/qwen3.8-27b': radixark/qwen3.8-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a870de8-45c492b818328ab509d8313e;1c5ad3de-e98a-44cc-b53e-20bb3853ebd2)

Repository Not Found for url: https://huggingface.co/radixark/qwen3.8-27b/resolve/main/tokenizer.json.
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
Average latency (api): 3.52 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |     t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:---------------------|------------:|----------------:|---------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| radixark/qwen3.8-27b | pp2048 (c4) | 2087.29 ± 95.71 | 527.49 ± 29.61 |              |                  | 3486.44 ± 118.08 | 3482.92 ± 118.08 | 3486.44 ± 118.08 |
| radixark/qwen3.8-27b |   tg32 (c4) |    49.04 ± 2.11 |   14.40 ± 1.73 | 60.67 ± 1.70 |     17.25 ± 2.38 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 16:23:35 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "radixark/qwen3.8-27b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 17:18:30
Benchmarking model: radixark/qwen3.8-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'radixark/qwen3.8-27b': radixark/qwen3.8-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a871ac7-0a7c672349a9b11d42b74966;fd8c5929-15a0-4894-bf33-8d39266d0b48)

Repository Not Found for url: https://huggingface.co/radixark/qwen3.8-27b/resolve/main/tokenizer.json.
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
Average latency (api): 3.25 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |    t/s (total) |     t/s (req) |     peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:---------------------|------------:|---------------:|--------------:|-------------:|-----------------:|----------------:|----------------:|----------------:|
| radixark/qwen3.8-27b | pp2048 (c4) | 1934.66 ± 1.87 | 488.45 ± 8.69 |              |                  | 3828.81 ± 83.14 | 3825.55 ± 83.14 | 3828.81 ± 83.14 |
| radixark/qwen3.8-27b |   tg32 (c4) |   48.71 ± 2.81 |  13.73 ± 1.03 | 61.33 ± 1.70 |     16.17 ± 1.21 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 17:18:30 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
