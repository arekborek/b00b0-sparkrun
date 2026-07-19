(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "jackrong/qwopus3.6-27b-coder" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 19:37:22
Benchmarking model: jackrong/qwopus3.6-27b-coder at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Probe) complete. Delta: 14 tokens (Server: 36, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 2.59 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                        |   test |           t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------------|-------:|--------------:|-------------:|---------------:|---------------:|----------------:|
| jackrong/qwopus3.6-27b-coder | pp2048 | 644.37 ± 1.04 |              | 3182.44 ± 5.15 | 3179.85 ± 5.15 |  3182.44 ± 5.15 |
| jackrong/qwopus3.6-27b-coder |   tg32 |  17.71 ± 2.01 | 19.00 ± 0.82 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 19:37:22 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "jackrong/qwopus3.6-27b-coder" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 19:37:52
Benchmarking model: jackrong/qwopus3.6-27b-coder at http://gx10-d2cf.local:4000/v1
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
Average latency (api): 4.44 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                        |   test |           t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------------|-------:|--------------:|-------------:|---------------:|---------------:|----------------:|
| jackrong/qwopus3.6-27b-coder | pp2048 | 642.24 ± 1.85 |              | 3195.36 ± 8.54 | 3190.92 ± 8.54 |  3195.36 ± 8.54 |
| jackrong/qwopus3.6-27b-coder |   tg32 |  17.50 ± 0.69 | 19.33 ± 1.25 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 19:37:52 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "jackrong/qwopus3.6-27b-coder" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 19:38:33
Benchmarking model: jackrong/qwopus3.6-27b-coder at http://gx10-d2cf.local:4000/v1
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
Average latency (api): 3.68 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                        |        test |   t/s (total) |     t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-----------------------------|------------:|--------------:|--------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| jackrong/qwopus3.6-27b-coder | pp2048 (c4) | 476.35 ± 0.61 | 119.42 ± 0.55 |              |                  | 17161.61 ± 77.89 | 17157.93 ± 77.89 | 17161.61 ± 77.89 |
| jackrong/qwopus3.6-27b-coder |   tg32 (c4) |  53.20 ± 6.14 |  16.83 ± 2.44 | 70.67 ± 5.31 |     19.50 ± 2.96 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 19:38:33 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "jackrong/qwopus3.6-27b-coder" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 19:40:08
Benchmarking model: jackrong/qwopus3.6-27b-coder at http://gx10-d2cf.local:4000/v1
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
Average latency (api): 4.52 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                        |        test |     t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |          ttfr (ms) |       est_ppt (ms) |      e2e_ttft (ms) |
|:-----------------------------|------------:|----------------:|---------------:|-------------:|-----------------:|-------------------:|-------------------:|-------------------:|
| jackrong/qwopus3.6-27b-coder | pp2048 (c4) | 590.01 ± 121.97 | 148.04 ± 30.74 |              |                  | 14402.39 ± 2698.41 | 14397.86 ± 2698.41 | 14402.39 ± 2698.41 |
| jackrong/qwopus3.6-27b-coder |   tg32 (c4) |    53.45 ± 1.43 |   15.80 ± 1.95 | 68.00 ± 4.55 |     17.92 ± 1.44 |                    |                    |                    |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 19:40:08 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
