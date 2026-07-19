(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwen3.6-35b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:05:22
Benchmarking model: qwen3.6-35b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwen3.6-35b': qwen3.6-35b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cbd82-64ad3af51d3235dc40308d9e;0c9a6ad2-e5d1-4f8d-9a24-3d3c0de14c87)

Repository Not Found for url: https://huggingface.co/qwen3.6-35b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.87 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model       |   test |             t/s |      peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:------------|-------:|----------------:|--------------:|--------------:|---------------:|----------------:|
| qwen3.6-35b | pp2048 | 4806.57 ± 99.03 |               | 399.37 ± 4.27 |  395.50 ± 4.27 |   399.37 ± 4.27 |
| qwen3.6-35b |   tg32 |   71.12 ± 13.06 | 73.41 ± 13.48 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:05:22 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwen3.6-35b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:05:33
Benchmarking model: qwen3.6-35b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwen3.6-35b': qwen3.6-35b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cbd8d-3b26e005560a881244db6bd0;adae6b4a-7c77-4cee-bf49-1542c7dd2e37)

Repository Not Found for url: https://huggingface.co/qwen3.6-35b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 5.37 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model       |   test |              t/s |     peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:------------|-------:|-----------------:|-------------:|--------------:|---------------:|----------------:|
| qwen3.6-35b | pp2048 | 4773.52 ± 164.23 |              | 390.52 ± 9.47 |  385.15 ± 9.47 |   390.52 ± 9.47 |
| qwen3.6-35b |   tg32 |     68.68 ± 8.30 | 70.89 ± 8.57 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:05:33 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwen3.6-35b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:05:42
Benchmarking model: qwen3.6-35b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwen3.6-35b': qwen3.6-35b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cbd96-21c8945b28961f4e68f03386;6335d827-c029-4b59-8ebb-df8a768bed3c)

Repository Not Found for url: https://huggingface.co/qwen3.6-35b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.57 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model       |        test |     t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:------------|------------:|----------------:|-----------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| qwen3.6-35b | pp2048 (c4) | 5804.61 ± 33.93 | 1526.47 ± 122.34 |               |                  | 1227.07 ± 91.07 | 1222.49 ± 91.07 | 1227.07 ± 91.07 |
| qwen3.6-35b |   tg32 (c4) |   139.04 ± 9.11 |     48.67 ± 6.22 | 143.53 ± 9.40 |     50.24 ± 6.42 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:05:42 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwen3.6-35b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:05:57
Benchmarking model: qwen3.6-35b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwen3.6-35b': qwen3.6-35b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cbda6-2a794ef6470e19b213b446eb;81946bab-590f-4834-95be-0879c51bf998)

Repository Not Found for url: https://huggingface.co/qwen3.6-35b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 5.05 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model       |        test |     t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:------------|------------:|----------------:|-----------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| qwen3.6-35b | pp2048 (c4) | 5869.27 ± 32.01 | 1542.37 ± 113.66 |               |                  | 1222.88 ± 88.23 | 1217.83 ± 88.23 | 1222.88 ± 88.23 |
| qwen3.6-35b |   tg32 (c4) |   139.95 ± 2.92 |     46.29 ± 7.28 | 144.47 ± 3.01 |     47.78 ± 7.51 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:05:57 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwen3.6-35b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:06:16
Benchmarking model: qwen3.6-35b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwen3.6-35b': qwen3.6-35b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cbdb9-2f18c87717467ebf73ca2a09;e3fbab56-4016-41fb-a69f-29e655261de5)

Repository Not Found for url: https://huggingface.co/qwen3.6-35b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 2.29 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model       |        test |     t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:------------|------------:|----------------:|-----------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| qwen3.6-35b | pp2048 (c4) | 5904.13 ± 24.90 | 1550.76 ± 133.44 |               |                  | 1221.06 ± 89.71 | 1218.76 ± 89.71 | 1221.06 ± 89.71 |
| qwen3.6-35b |   tg32 (c4) |   136.01 ± 1.57 |    48.95 ± 11.28 | 140.40 ± 1.62 |    50.53 ± 11.64 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:06:16 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwen3.6-35b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 14:09:23
Benchmarking model: qwen3.6-35b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwen3.6-35b': qwen3.6-35b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cbe73-1fe0d6234116d1331a2c6074;71646686-f93e-496f-b715-734ff2a62cd7)

Repository Not Found for url: https://huggingface.co/qwen3.6-35b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.16 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model       |        test |     t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:------------|------------:|----------------:|-----------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| qwen3.6-35b | pp2048 (c4) | 5890.91 ± 25.67 | 1546.82 ± 125.29 |               |                  | 1219.87 ± 87.55 | 1216.72 ± 87.55 | 1219.87 ± 87.55 |
| qwen3.6-35b |   tg32 (c4) |   137.47 ± 3.37 |     46.62 ± 5.00 | 141.91 ± 3.48 |     48.13 ± 5.16 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 14:09:23 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
