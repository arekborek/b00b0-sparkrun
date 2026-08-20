(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/muse-glimmer-30b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 15:21:43
Benchmarking model: redhatai/muse-glimmer-30b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
tokenizer.json: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 28.1M/28.1M [00:03<00:00, 8.70MB/s]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 143636
Warming up...
Warmup (User only) complete. Delta: 22 tokens (Server: 43, Local: 21)
Warmup (System+Probe) complete. Delta: 34 tokens (Server: 56, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 5.40 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                     |        test |     t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:--------------------------|------------:|----------------:|---------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| redhatai/muse-glimmer-30b | pp2048 (c4) | 2044.73 ± 34.36 | 517.79 ± 13.50 |              |                  | 3964.96 ± 101.68 | 3959.56 ± 101.68 | 3964.96 ± 101.68 |
| redhatai/muse-glimmer-30b |   tg32 (c4) |    40.12 ± 1.03 |   13.45 ± 4.23 | 57.00 ± 6.16 |     16.00 ± 4.20 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 15:21:43 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/muse-glimmer-30b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 15:22:24
Benchmarking model: redhatai/muse-glimmer-30b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 143636
Warming up...
Warmup (User only) complete. Delta: 22 tokens (Server: 43, Local: 21)
Warmup (System+Probe) complete. Delta: 34 tokens (Server: 56, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.41 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                     |        test |     t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------------|------------:|----------------:|---------------:|-------------:|-----------------:|----------------:|----------------:|----------------:|
| redhatai/muse-glimmer-30b | pp2048 (c4) | 2054.60 ± 25.66 | 520.17 ± 12.24 |              |                  | 3944.68 ± 92.26 | 3941.27 ± 92.26 | 3944.68 ± 92.26 |
| redhatai/muse-glimmer-30b |   tg32 (c4) |    43.06 ± 2.03 |   12.93 ± 1.05 | 58.00 ± 2.83 |     16.42 ± 1.61 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 15:22:24 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/muse-glimmer-30b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 15:28:01
Benchmarking model: redhatai/muse-glimmer-30b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 143636
Warming up...
Warmup (User only) complete. Delta: 22 tokens (Server: 43, Local: 21)
Warmup (System+Probe) complete. Delta: 34 tokens (Server: 56, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.12 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                     |        test |     t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------------|------------:|----------------:|---------------:|-------------:|-----------------:|----------------:|----------------:|----------------:|
| redhatai/muse-glimmer-30b | pp2048 (c4) | 2050.31 ± 26.69 | 519.01 ± 12.25 |              |                  | 3953.68 ± 91.74 | 3949.56 ± 91.74 | 3953.68 ± 91.74 |
| redhatai/muse-glimmer-30b |   tg32 (c4) |    45.13 ± 1.26 |   13.66 ± 3.92 | 60.00 ± 4.55 |     16.75 ± 4.42 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 15:28:01 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/muse-glimmer-30b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 15:28:51
Benchmarking model: redhatai/muse-glimmer-30b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 143636
Warming up...
Warmup (User only) complete. Delta: 22 tokens (Server: 43, Local: 21)
Warmup (System+Probe) complete. Delta: 34 tokens (Server: 56, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.25 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                     |   test |            t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------------|-------:|---------------:|-------------:|---------------:|---------------:|----------------:|
| redhatai/muse-glimmer-30b | pp2048 | 1687.14 ± 2.90 |              | 1218.74 ± 2.09 | 1214.48 ± 2.09 |  1218.74 ± 2.09 |
| redhatai/muse-glimmer-30b |   tg32 |   13.90 ± 3.27 | 16.33 ± 3.30 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 15:28:51 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/muse-glimmer-30b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-08-20 15:29:14
Benchmarking model: redhatai/muse-glimmer-30b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 143636
Warming up...
Warmup (User only) complete. Delta: 22 tokens (Server: 43, Local: 21)
Warmup (System+Probe) complete. Delta: 34 tokens (Server: 56, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.51 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                     |   test |             t/s |     peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------------|-------:|----------------:|-------------:|----------------:|----------------:|----------------:|
| redhatai/muse-glimmer-30b | pp2048 | 1747.06 ± 94.81 |              | 1180.50 ± 61.75 | 1175.99 ± 61.75 | 1180.50 ± 61.75 |
| redhatai/muse-glimmer-30b |   tg32 |    18.55 ± 5.89 | 21.00 ± 5.89 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-08-20 15:29:14 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
