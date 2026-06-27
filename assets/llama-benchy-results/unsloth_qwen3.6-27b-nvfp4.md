(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "unsloth/qwen3.6-27b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:56:58
Benchmarking model: unsloth/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
config.json: 3.70kB [00:00, 6.91MB/s]
tokenizer_config.json: 15.8kB [00:00, 36.6MB/s]
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
vocab.json: 5.23MB [00:01, 4.03MB/s]
merges.txt: 3.35MB [00:01, 3.29MB/s]
tokenizer.json: 100%|█████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 20.0M/20.0M [00:11<00:00, 1.75MB/s]
added_tokens.json: 100%|██████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 904/904 [00:00<00:00, 1.30MB/s]
special_tokens_map.json: 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 876/876 [00:00<00:00, 2.43MB/s]
chat_template.jinja: 8.06kB [00:00, 8.85MB/s]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.54 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model               |   test |             t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------|-------:|----------------:|-------------:|---------------:|---------------:|----------------:|
| unsloth/qwen3.6-27b | pp2048 | 1880.34 ± 12.42 |              | 1094.28 ± 7.22 | 1089.75 ± 7.22 |  1094.28 ± 7.22 |
| unsloth/qwen3.6-27b |   tg32 |    21.92 ± 1.31 | 23.33 ± 0.47 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:56:58 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "unsloth/qwen3.6-27b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:57:44
Benchmarking model: unsloth/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.02 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model               |   test |            t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------|-------:|---------------:|-------------:|---------------:|---------------:|----------------:|
| unsloth/qwen3.6-27b | pp2048 | 1867.20 ± 4.09 |              | 1101.57 ± 2.39 | 1097.55 ± 2.39 |  1101.57 ± 2.39 |
| unsloth/qwen3.6-27b |   tg32 |   21.32 ± 1.95 | 24.00 ± 1.41 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:57:44 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "unsloth/qwen3.6-27b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:58:10
Benchmarking model: unsloth/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
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
Average latency (api): 2.85 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model               |        test |     t/s (total) |     t/s (req) |     peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------|------------:|----------------:|--------------:|-------------:|-----------------:|----------------:|----------------:|----------------:|
| unsloth/qwen3.6-27b | pp2048 (c4) | 1804.35 ± 22.07 | 451.42 ± 5.53 |              |                  | 4542.95 ± 55.38 | 4540.09 ± 55.38 | 4542.95 ± 55.38 |
| unsloth/qwen3.6-27b |   tg32 (c4) |    78.22 ± 4.20 |  21.49 ± 1.65 | 96.33 ± 2.87 |     24.08 ± 1.11 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:58:10 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "unsloth/qwen3.6-27b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:58:51
Benchmarking model: unsloth/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 144480
Warming up...
Warmup (User only) complete. Delta: 9 tokens (Server: 30, Local: 21)
Warmup (System+Empty) complete. Delta: 14 tokens (Server: 35, Local: 21)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.27 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model               |        test |     t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:--------------------|------------:|----------------:|---------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| unsloth/qwen3.6-27b | pp2048 (c4) | 2028.61 ± 63.81 | 520.00 ± 18.00 |              |                  | 3947.74 ± 136.86 | 3944.47 ± 136.86 | 3947.74 ± 136.86 |
| unsloth/qwen3.6-27b |   tg32 (c4) |    70.72 ± 6.20 |   21.53 ± 2.35 | 94.00 ± 2.16 |     24.17 ± 1.07 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:58:51 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
