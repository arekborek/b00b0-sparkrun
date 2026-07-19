(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "deepreinforce-ai/ornith-1.0-35b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:11:17
Benchmarking model: deepreinforce-ai/ornith-1.0-35b at http://gx10-d2cf.local:4000/v1
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
Average latency (api): 4.78 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                           |   test |             t/s |     peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------------------|-------:|----------------:|-------------:|--------------:|---------------:|----------------:|
| deepreinforce-ai/ornith-1.0-35b | pp2048 | 4951.90 ± 34.11 |              | 418.58 ± 2.84 |  413.80 ± 2.84 |   418.58 ± 2.84 |
| deepreinforce-ai/ornith-1.0-35b |   tg32 |    39.65 ± 0.06 | 40.92 ± 0.06 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:11:17 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "deepreinforce-ai/ornith-1.0-35b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:11:30
Benchmarking model: deepreinforce-ai/ornith-1.0-35b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Probe) complete. Delta: 14 tokens (Server: 36, Local context: 21, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.65 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                           |   test |             t/s |     peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------------------|-------:|----------------:|-------------:|--------------:|---------------:|----------------:|
| deepreinforce-ai/ornith-1.0-35b | pp2048 | 4921.05 ± 38.09 |              | 421.11 ± 3.30 |  416.47 ± 3.30 |   421.11 ± 3.30 |
| deepreinforce-ai/ornith-1.0-35b |   tg32 |    39.61 ± 0.08 | 40.89 ± 0.09 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:11:30 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "deepreinforce-ai/ornith-1.0-35b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:11:43
Benchmarking model: deepreinforce-ai/ornith-1.0-35b at http://gx10-d2cf.local:4000/v1
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
Average latency (api): 4.20 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                           |        test |     t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:--------------------------------|------------:|----------------:|-----------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| deepreinforce-ai/ornith-1.0-35b | pp2048 (c4) | 5937.28 ± 17.95 | 1743.53 ± 440.50 |               |                  | 1240.53 ± 241.76 | 1236.33 ± 241.76 | 1240.53 ± 241.76 |
| deepreinforce-ai/ornith-1.0-35b |   tg32 (c4) |    80.60 ± 2.07 |     28.91 ± 4.90 | 126.00 ± 1.41 |     32.18 ± 1.44 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:11:43 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "deepreinforce-ai/ornith-1.0-35b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:12:20
Benchmarking model: deepreinforce-ai/ornith-1.0-35b at http://gx10-d2cf.local:4000/v1
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
Average latency (api): 3.41 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                           |        test |     t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:--------------------------------|------------:|----------------:|-----------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| deepreinforce-ai/ornith-1.0-35b | pp2048 (c4) | 5920.54 ± 12.12 | 1739.14 ± 441.73 |               |                  | 1243.43 ± 243.54 | 1240.02 ± 243.54 | 1243.43 ± 243.54 |
| deepreinforce-ai/ornith-1.0-35b |   tg32 (c4) |    79.69 ± 1.24 |     28.52 ± 4.71 | 125.00 ± 1.41 |     31.57 ± 0.99 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:12:20 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
