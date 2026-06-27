(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "prisma_scout/qwen3.6-27b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:26:11
Benchmarking model: prisma_scout/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: prisma_scout/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.24 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                    |   test |              t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------------|-------:|-----------------:|-------------:|---------------:|---------------:|----------------:|
| prisma_scout/qwen3.6-27b | pp2048 | 1944.43 ± 103.98 |              | 984.13 ± 79.67 | 980.89 ± 79.67 |  984.13 ± 79.67 |
| prisma_scout/qwen3.6-27b |   tg32 |     25.94 ± 2.36 | 28.33 ± 0.94 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:26:11 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "prisma_scout/qwen3.6-27b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:26:30
Benchmarking model: prisma_scout/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: prisma_scout/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 2.81 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                    |   test |              t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------------|-------:|-----------------:|-------------:|---------------:|---------------:|----------------:|
| prisma_scout/qwen3.6-27b | pp2048 | 1939.78 ± 101.06 |              | 960.79 ± 69.41 | 957.98 ± 69.41 |  960.79 ± 69.41 |
| prisma_scout/qwen3.6-27b |   tg32 |     25.85 ± 2.31 | 27.33 ± 2.05 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:26:30 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "prisma_scout/qwen3.6-27b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:26:50
Benchmarking model: prisma_scout/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: prisma_scout/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.57 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                    |        test |     t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------------|------------:|----------------:|---------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| prisma_scout/qwen3.6-27b | pp2048 (c4) | 2358.42 ± 13.40 | 600.91 ± 23.05 |               |                  | 3121.94 ± 78.74 | 3118.37 ± 78.74 | 3121.94 ± 78.74 |
| prisma_scout/qwen3.6-27b |   tg32 (c4) |    88.80 ± 2.47 |   23.80 ± 1.94 | 106.33 ± 2.62 |     26.67 ± 1.70 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:26:50 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "prisma_scout/qwen3.6-27b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:27:18
Benchmarking model: prisma_scout/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: prisma_scout/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.15 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                    |        test |    t/s (total) |     t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------------|------------:|---------------:|--------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| prisma_scout/qwen3.6-27b | pp2048 (c4) | 2367.11 ± 4.95 | 592.46 ± 6.78 |               |                  | 3159.36 ± 46.49 | 3156.21 ± 46.49 | 3159.36 ± 46.49 |
| prisma_scout/qwen3.6-27b |   tg32 (c4) |   96.83 ± 3.79 |  25.55 ± 1.51 | 110.33 ± 1.25 |     27.58 ± 1.38 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:27:18 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
