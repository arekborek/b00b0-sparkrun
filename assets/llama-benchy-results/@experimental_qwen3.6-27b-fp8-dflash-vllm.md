(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 11:35:23
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Probe) complete. Delta: 14 tokens (Server: 36, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 5.15 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                |   test |            t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:---------------------|-------:|---------------:|-------------:|---------------:|---------------:|----------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 | 1374.19 ± 4.17 |              | 1496.22 ± 4.52 | 1491.07 ± 4.52 |  1496.22 ± 4.52 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 |   32.89 ± 4.53 | 34.77 ± 3.79 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 11:35:23 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 11:35:39
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Probe) complete. Delta: 14 tokens (Server: 36, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.50 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                |   test |             t/s |     peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:---------------------|-------:|----------------:|-------------:|----------------:|----------------:|----------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 | 1598.75 ± 98.85 |              | 1290.65 ± 76.47 | 1286.14 ± 76.47 | 1290.65 ± 76.47 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 |    30.80 ± 2.15 | 32.57 ± 1.11 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 11:35:39 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 11:35:55
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
^[[AWarmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Probe) complete. Delta: 14 tokens (Server: 36, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 2.53 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |     t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |         ttfr (ms) |      est_ppt (ms) |     e2e_ttft (ms) |
|:---------------------|------------:|----------------:|---------------:|--------------:|-----------------:|------------------:|------------------:|------------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 (c4) | 980.05 ± 276.53 | 247.54 ± 69.27 |               |                  | 8982.37 ± 2560.29 | 8979.84 ± 2560.29 | 8982.37 ± 2560.29 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 (c4) |   71.62 ± 16.68 |   23.54 ± 3.38 | 112.33 ± 5.44 |     28.58 ± 1.66 |                   |                   |                   |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 11:35:55 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 11:55:56
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Probe) complete. Delta: 14 tokens (Server: 36, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.28 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |     t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |         ttfr (ms) |      est_ppt (ms) |     e2e_ttft (ms) |
|:---------------------|------------:|----------------:|---------------:|--------------:|-----------------:|------------------:|------------------:|------------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 (c4) | 983.29 ± 277.76 | 248.38 ± 69.60 |               |                  | 8957.31 ± 2562.62 | 8954.03 ± 2562.62 | 8957.31 ± 2562.62 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 (c4) |   71.69 ± 18.01 |   24.92 ± 4.08 | 110.33 ± 7.59 |     28.00 ± 3.16 |                   |                   |                   |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 11:55:56 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Qwen/Qwen3.6-27B-FP8" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 11:57:40
Benchmarking model: Qwen/Qwen3.6-27B-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Probe) complete. Delta: 14 tokens (Server: 36, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.79 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                |        test |    t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |         ttfr (ms) |      est_ppt (ms) |     e2e_ttft (ms) |
|:---------------------|------------:|---------------:|---------------:|--------------:|-----------------:|------------------:|------------------:|------------------:|
| Qwen/Qwen3.6-27B-FP8 | pp2048 (c4) | 678.24 ± 18.90 | 172.96 ± 13.74 |               |                  | 11914.18 ± 792.53 | 11909.39 ± 792.53 | 11914.18 ± 792.53 |
| Qwen/Qwen3.6-27B-FP8 |   tg32 (c4) |  65.66 ± 21.23 |   23.78 ± 5.89 | 112.33 ± 5.44 |     28.56 ± 4.19 |                   |                   |                   |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 11:57:40 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
