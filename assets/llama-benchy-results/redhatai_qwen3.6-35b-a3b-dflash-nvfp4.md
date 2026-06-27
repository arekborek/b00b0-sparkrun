(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/qwen3.6-35b-a3b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:40:20
Benchmarking model: redhatai/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: redhatai/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 4.89 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                    |   test |             t/s |       peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------------|-------:|----------------:|---------------:|--------------:|---------------:|----------------:|
| redhatai/qwen3.6-35b-a3b | pp2048 | 5239.10 ± 93.89 |                | 363.64 ± 9.34 |  358.74 ± 9.34 |   363.64 ± 9.34 |
| redhatai/qwen3.6-35b-a3b |   tg32 |  113.98 ± 27.78 | 117.74 ± 28.73 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:40:20 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/qwen3.6-35b-a3b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:41:59
Benchmarking model: redhatai/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: redhatai/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.52 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                    |   test |             t/s |      peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------------|-------:|----------------:|--------------:|--------------:|---------------:|----------------:|
| redhatai/qwen3.6-35b-a3b | pp2048 | 5156.29 ± 44.19 |               | 367.43 ± 3.94 |  363.91 ± 3.94 |   367.43 ± 3.94 |
| redhatai/qwen3.6-35b-a3b |   tg32 |   124.61 ± 1.43 | 128.72 ± 1.48 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:41:59 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/qwen3.6-35b-a3b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:42:10
Benchmarking model: redhatai/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: redhatai/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 4.30 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                    |        test |     t/s (total) |        t/s (req) |       peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-------------------------|------------:|----------------:|-----------------:|---------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| redhatai/qwen3.6-35b-a3b | pp2048 (c4) | 6034.52 ± 56.98 | 1715.44 ± 287.92 |                |                  | 1108.95 ± 157.73 | 1104.65 ± 157.73 | 1108.95 ± 157.73 |
| redhatai/qwen3.6-35b-a3b |   tg32 (c4) |  165.28 ± 50.90 |    70.49 ± 17.50 | 173.86 ± 49.34 |    72.79 ± 18.07 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:42:10 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "redhatai/qwen3.6-35b-a3b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:42:30
Benchmarking model: redhatai/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: redhatai/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 2.57 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                    |        test |      t/s (total) |        t/s (req) |       peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-------------------------|------------:|-----------------:|-----------------:|---------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| redhatai/qwen3.6-35b-a3b | pp2048 (c4) | 6221.23 ± 314.18 | 1693.61 ± 293.66 |                |                  | 1123.56 ± 152.92 | 1120.99 ± 152.92 | 1123.56 ± 152.92 |
| redhatai/qwen3.6-35b-a3b |   tg32 (c4) |   166.30 ± 53.31 |    68.61 ± 17.50 | 171.66 ± 55.03 |    70.85 ± 18.08 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:42:30 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
