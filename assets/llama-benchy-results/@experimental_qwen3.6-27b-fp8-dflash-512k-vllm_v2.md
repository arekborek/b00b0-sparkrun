(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-25 16:48:53
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
Average latency (api): 3.72 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |     t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |          ttfr (ms) |       est_ppt (ms) |      e2e_ttft (ms) |
|:---------------------|------------:|----------------:|---------------:|--------------:|-----------------:|-------------------:|-------------------:|-------------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 (c4) | 816.29 ± 251.97 | 207.28 ± 61.94 |               |                  | 10705.99 ± 2747.07 | 10702.27 ± 2747.07 | 10705.99 ± 2747.07 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 (c4) |   66.35 ± 22.73 |   23.96 ± 5.98 | 109.67 ± 7.13 |     27.79 ± 4.61 |                    |                    |                    |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-25 16:48:53 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-25 17:11:15
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
Average latency (api): 3.32 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |     t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |          ttfr (ms) |       est_ppt (ms) |      e2e_ttft (ms) |
|:---------------------|------------:|----------------:|---------------:|--------------:|-----------------:|-------------------:|-------------------:|-------------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 (c4) | 816.83 ± 249.96 | 207.42 ± 61.42 |               |                  | 10682.89 ± 2716.82 | 10679.57 ± 2716.82 | 10682.89 ± 2716.82 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 (c4) |   63.68 ± 21.92 |   22.31 ± 4.49 | 115.67 ± 2.05 |     28.92 ± 0.86 |                    |                    |                    |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-25 17:11:15 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-25 17:14:06
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
Average latency (api): 4.10 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |     t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |         ttfr (ms) |      est_ppt (ms) |     e2e_ttft (ms) |
|:---------------------|------------:|----------------:|---------------:|--------------:|-----------------:|------------------:|------------------:|------------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 (c4) | 984.62 ± 257.68 | 246.30 ± 64.48 |               |                  | 9087.92 ± 2919.16 | 9083.82 ± 2919.16 | 9087.92 ± 2919.16 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 (c4) |    87.64 ± 5.46 |   27.17 ± 5.48 | 118.67 ± 2.05 |     30.82 ± 3.48 |                   |                   |                   |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-25 17:14:06 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
