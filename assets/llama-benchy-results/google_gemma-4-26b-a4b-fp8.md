(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "google/gemma-4-26b-a4b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 21:51:18
Benchmarking model: google/gemma-4-26b-a4b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
config.json: 3.77kB [00:00, 6.32MB/s]
tokenizer_config.json: 100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 881/881 [00:00<00:00, 2.83MB/s]
tokenizer.json: 100%|█████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 32.2M/32.2M [00:03<00:00, 8.88MB/s]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144040
Warming up...
Warmup (User only) complete. Delta: 12 tokens (Server: 33, Local: 21)
Warmup (System+Empty) complete. Delta: 18 tokens (Server: 39, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.38 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |              t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|-----------------:|-------------:|---------------:|---------------:|----------------:|
| google/gemma-4-26b-a4b | pp2048 | 5774.92 ± 578.60 |              | 362.99 ± 38.55 | 358.61 ± 38.55 |  362.99 ± 38.55 |
| google/gemma-4-26b-a4b |   tg32 |     40.23 ± 0.06 | 41.54 ± 0.06 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 21:51:18 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "google/gemma-4-26b-a4b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 21:51:41
Benchmarking model: google/gemma-4-26b-a4b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144040
Warming up...
Warmup (User only) complete. Delta: 12 tokens (Server: 33, Local: 21)
Warmup (System+Empty) complete. Delta: 18 tokens (Server: 39, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 2.83 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |             t/s |     peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|----------------:|-------------:|--------------:|---------------:|----------------:|
| google/gemma-4-26b-a4b | pp2048 | 6210.01 ± 61.47 |              | 332.86 ± 3.18 |  330.04 ± 3.18 |   332.86 ± 3.18 |
| google/gemma-4-26b-a4b |   tg32 |    39.90 ± 0.04 | 41.19 ± 0.05 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 21:51:41 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "google/gemma-4-26b-a4b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 21:51:54
Benchmarking model: google/gemma-4-26b-a4b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144040
Warming up...
Warmup (User only) complete. Delta: 12 tokens (Server: 33, Local: 21)
Warmup (System+Empty) complete. Delta: 18 tokens (Server: 39, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.98 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |     t/s (total) |         t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-----------------------|------------:|----------------:|------------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| google/gemma-4-26b-a4b | pp2048 (c4) | 6710.19 ± 95.05 | 2218.87 ± 1178.58 |               |                  | 1055.38 ± 256.29 | 1051.40 ± 256.29 | 1055.38 ± 256.29 |
| google/gemma-4-26b-a4b |   tg32 (c4) |   77.48 ± 15.02 |      22.59 ± 2.88 | 100.00 ± 0.00 |     25.08 ± 0.28 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 21:51:54 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "google/gemma-4-26b-a4b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 21:52:10
Benchmarking model: google/gemma-4-26b-a4b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144040
Warming up...
Warmup (User only) complete. Delta: 12 tokens (Server: 33, Local: 21)
Warmup (System+Empty) complete. Delta: 18 tokens (Server: 39, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.36 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |      t/s (total) |         t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-----------------------|------------:|-----------------:|------------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| google/gemma-4-26b-a4b | pp2048 (c4) | 6796.10 ± 133.59 | 2233.21 ± 1187.12 |               |                  | 1048.69 ± 256.25 | 1045.32 ± 256.25 | 1048.69 ± 256.25 |
| google/gemma-4-26b-a4b |   tg32 (c4) |    77.11 ± 14.19 |      22.48 ± 2.96 | 100.33 ± 2.87 |     25.08 ± 0.76 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 21:52:10 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
