(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "jackrong/qwopus3.6-27b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 13:55:16
Benchmarking model: jackrong/qwopus3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: jackrong/qwopus3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>`
Falling back to 'gpt2' tokenizer as approximation.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
[transformers] Token indices sequence length is longer than the specified maximum sequence length for this model (159385 > 1024). Running this sequence through the model will result in indexing errors
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Empty) complete. Delta: 13 tokens (Server: 35, Local: 22)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 5.26 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |           t/s |     peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|--------------:|-------------:|----------------:|----------------:|----------------:|
| jackrong/qwopus3.6-27b | pp2048 | 595.22 ± 2.52 |              | 3152.16 ± 75.04 | 3146.90 ± 75.04 | 3152.16 ± 75.04 |
| jackrong/qwopus3.6-27b |   tg32 |  18.07 ± 1.76 | 18.67 ± 1.25 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 13:55:16 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "jackrong/qwopus3.6-27b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 14:10:38
Benchmarking model: jackrong/qwopus3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: jackrong/qwopus3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>`
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
[transformers] Token indices sequence length is longer than the specified maximum sequence length for this model (159385 > 1024). Running this sequence through the model will result in indexing errors
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Empty) complete. Delta: 13 tokens (Server: 35, Local: 22)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 2.91 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |           t/s |     peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|--------------:|-------------:|----------------:|----------------:|----------------:|
| jackrong/qwopus3.6-27b | pp2048 | 583.87 ± 8.08 |              | 3210.11 ± 12.47 | 3207.20 ± 12.47 | 3210.11 ± 12.47 |
| jackrong/qwopus3.6-27b |   tg32 |  14.59 ± 1.63 | 16.33 ± 1.25 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 14:10:38 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "jackrong/qwopus3.6-27b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 14:11:17
Benchmarking model: jackrong/qwopus3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: jackrong/qwopus3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>`
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
[transformers] Token indices sequence length is longer than the specified maximum sequence length for this model (159385 > 1024). Running this sequence through the model will result in indexing errors
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Empty) complete. Delta: 13 tokens (Server: 35, Local: 22)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.30 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |     t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |          ttfr (ms) |       est_ppt (ms) |      e2e_ttft (ms) |
|:-----------------------|------------:|----------------:|---------------:|-------------:|-----------------:|-------------------:|-------------------:|-------------------:|
| jackrong/qwopus3.6-27b | pp2048 (c4) | 692.16 ± 172.55 | 175.07 ± 44.34 |              |                  | 11507.80 ± 3501.46 | 11504.50 ± 3501.46 | 11507.80 ± 3501.46 |
| jackrong/qwopus3.6-27b |   tg32 (c4) |    58.77 ± 2.15 |   16.29 ± 1.41 | 68.67 ± 5.91 |     18.17 ± 1.28 |                    |                    |                    |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 14:11:17 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "jackrong/qwopus3.6-27b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 14:22:32
Benchmarking model: jackrong/qwopus3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: jackrong/qwopus3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>`
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
[transformers] Token indices sequence length is longer than the specified maximum sequence length for this model (159385 > 1024). Running this sequence through the model will result in indexing errors
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Empty) complete. Delta: 13 tokens (Server: 35, Local: 22)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.07 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |    t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |          ttfr (ms) |       est_ppt (ms) |      e2e_ttft (ms) |
|:-----------------------|------------:|---------------:|---------------:|-------------:|-----------------:|-------------------:|-------------------:|-------------------:|
| jackrong/qwopus3.6-27b | pp2048 (c4) | 487.94 ± 56.62 | 122.77 ± 14.55 |              |                  | 15269.72 ± 1781.17 | 15265.64 ± 1781.17 | 15269.72 ± 1781.17 |
| jackrong/qwopus3.6-27b |   tg32 (c4) |  48.93 ± 12.07 |   14.38 ± 2.55 | 61.33 ± 8.81 |     17.00 ± 2.35 |                    |                    |                    |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 14:22:32 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
