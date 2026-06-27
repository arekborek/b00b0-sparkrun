arek@DESKTOP-15MQGOE llama-benchy % source .venv/bin/activate                   
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Jackrong/Qwopus3.6-27B-Coder-FP8" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-25 15:25:26
Benchmarking model: Jackrong/Qwopus3.6-27B-Coder-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
config.json: 51.7kB [00:00, 68.1MB/s]
tokenizer_config.json: 12.1kB [00:00, 18.2MB/s]
tokenizer.json: 100%|██████████████████████████████████████████████████████████████| 20.0M/20.0M [00:02<00:00, 9.07MB/s]
chat_template.jinja: 4.72kB [00:00, 7.97MB/s]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.99 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                            |        test |     t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |          ttfr (ms) |       est_ppt (ms) |      e2e_ttft (ms) |
|:---------------------------------|------------:|----------------:|---------------:|-------------:|-----------------:|-------------------:|-------------------:|-------------------:|
| Jackrong/Qwopus3.6-27B-Coder-FP8 | pp2048 (c4) | 596.67 ± 134.95 | 149.69 ± 33.99 |              |                  | 14347.93 ± 2910.60 | 14343.94 ± 2910.60 | 14347.93 ± 2910.60 |
| Jackrong/Qwopus3.6-27B-Coder-FP8 |   tg32 (c4) |    51.81 ± 3.15 |   14.77 ± 1.21 | 63.67 ± 2.49 |     17.08 ± 1.26 |                    |                    |                    |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-25 15:25:26 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Jackrong/Qwopus3.6-27B-Coder-FP8" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-25 15:27:03
Benchmarking model: Jackrong/Qwopus3.6-27B-Coder-FP8 at http://gx10-d2cf.local:4000/v1
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
Average latency (api): 4.40 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                            |        test |   t/s (total) |     t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:---------------------------------|------------:|--------------:|--------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| Jackrong/Qwopus3.6-27B-Coder-FP8 | pp2048 (c4) | 469.54 ± 0.33 | 117.69 ± 0.47 |              |                  | 17416.66 ± 69.56 | 17412.26 ± 69.56 | 17416.66 ± 69.56 |
| Jackrong/Qwopus3.6-27B-Coder-FP8 |   tg32 (c4) |  54.00 ± 1.57 |  15.17 ± 0.88 | 64.67 ± 2.36 |     18.00 ± 1.22 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-25 15:27:03 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "Jackrong/Qwopus3.6-27B-Coder-FP8" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-25 15:29:28
Benchmarking model: Jackrong/Qwopus3.6-27B-Coder-FP8 at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.21 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                            |        test |   t/s (total) |     t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:---------------------------------|------------:|--------------:|--------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| Jackrong/Qwopus3.6-27B-Coder-FP8 | pp2048 (c4) | 470.27 ± 0.30 | 117.86 ± 0.46 |              |                  | 17385.93 ± 70.29 | 17382.71 ± 70.29 | 17385.93 ± 70.29 |
| Jackrong/Qwopus3.6-27B-Coder-FP8 |   tg32 (c4) |  56.47 ± 3.05 |  16.38 ± 1.10 | 70.00 ± 1.41 |     18.17 ± 1.07 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-25 15:29:28 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
