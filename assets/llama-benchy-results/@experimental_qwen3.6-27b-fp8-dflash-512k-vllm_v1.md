(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 22:01:21
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 5.36 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                |   test |              t/s |     peak t/s |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:---------------------|-------:|-----------------:|-------------:|-----------------:|-----------------:|-----------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 | 1455.33 ± 143.28 |              | 1426.62 ± 138.02 | 1421.25 ± 138.02 | 1426.62 ± 138.02 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 |     24.92 ± 1.59 | 29.33 ± 0.94 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 22:01:21 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 22:02:22
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.11 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                |   test |             t/s |     peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:---------------------|-------:|----------------:|-------------:|----------------:|----------------:|----------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 | 1336.82 ± 64.45 |              | 1539.30 ± 71.64 | 1536.19 ± 71.64 | 1539.30 ± 71.64 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 |    28.86 ± 2.01 | 30.67 ± 0.47 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 22:02:22 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 22:02:44
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.01 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |   t/s (total) |     t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:---------------------|------------:|--------------:|--------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 (c4) | 605.14 ± 1.20 | 151.33 ± 0.30 |               |                  | 13542.79 ± 28.07 | 13539.78 ± 28.07 | 13542.79 ± 28.07 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 (c4) | 82.59 ± 12.22 |  24.90 ± 4.40 | 113.67 ± 1.70 |     28.69 ± 2.50 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 22:02:44 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 22:03:56
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.71 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |     t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |          ttfr (ms) |       est_ppt (ms) |      e2e_ttft (ms) |
|:---------------------|------------:|----------------:|---------------:|--------------:|-----------------:|-------------------:|-------------------:|-------------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 (c4) | 812.15 ± 295.64 | 203.13 ± 73.98 |               |                  | 11280.57 ± 3266.06 | 11276.86 ± 3266.06 | 11280.57 ± 3266.06 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 (c4) |   90.71 ± 14.93 |   25.68 ± 2.81 | 116.67 ± 2.87 |     29.17 ± 1.34 |                    |                    |                    |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 22:03:56 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
