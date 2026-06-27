(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/gemma-4-31b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 22:41:16
Benchmarking model: nvidia/gemma-4-31b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: nvidia/gemma-4-31b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>`
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
[transformers] Token indices sequence length is longer than the specified maximum sequence length for this model (159385 > 1024). Running this sequence through the model will result in indexing errors
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 11 tokens (Server: 33, Local: 22)
Warmup (System+Empty) complete. Delta: 17 tokens (Server: 39, Local: 22)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.02 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model              |   test |             t/s |    peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------|-------:|----------------:|------------:|----------------:|----------------:|----------------:|
| nvidia/gemma-4-31b | pp2048 | 1763.35 ± 84.80 |             | 1084.19 ± 50.66 | 1081.17 ± 50.66 | 1084.19 ± 50.66 |
| nvidia/gemma-4-31b |   tg32 |     6.79 ± 0.00 | 7.00 ± 0.00 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 22:41:16 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/gemma-4-31b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 22:41:44
Benchmarking model: nvidia/gemma-4-31b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: nvidia/gemma-4-31b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>`
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
[transformers] Token indices sequence length is longer than the specified maximum sequence length for this model (159385 > 1024). Running this sequence through the model will result in indexing errors
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 11 tokens (Server: 33, Local: 22)
Warmup (System+Empty) complete. Delta: 17 tokens (Server: 39, Local: 22)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 2.10 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model              |   test |            t/s |    peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------|-------:|---------------:|------------:|----------------:|----------------:|----------------:|
| nvidia/gemma-4-31b | pp2048 | 1816.60 ± 7.15 |             | 1034.76 ± 11.81 | 1032.66 ± 11.81 | 1034.76 ± 11.81 |
| nvidia/gemma-4-31b |   tg32 |    6.78 ± 0.00 | 7.00 ± 0.00 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 22:41:44 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/gemma-4-31b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 22:42:29
Benchmarking model: nvidia/gemma-4-31b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: nvidia/gemma-4-31b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>`
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
[transformers] Token indices sequence length is longer than the specified maximum sequence length for this model (159385 > 1024). Running this sequence through the model will result in indexing errors
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 11 tokens (Server: 33, Local: 22)
Warmup (System+Empty) complete. Delta: 17 tokens (Server: 39, Local: 22)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 2.81 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model              |        test |     t/s (total) |       t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-------------------|------------:|----------------:|----------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| nvidia/gemma-4-31b | pp2048 (c4) | 1764.03 ± 10.84 | 587.12 ± 151.87 |              |                  | 3311.88 ± 728.25 | 3309.07 ± 728.25 | 3311.88 ± 728.25 |
| nvidia/gemma-4-31b |   tg32 (c4) |    20.35 ± 1.70 |     5.71 ± 0.63 | 28.00 ± 0.00 |      7.00 ± 0.00 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 22:42:29 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/gemma-4-31b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 22:43:22
Benchmarking model: nvidia/gemma-4-31b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: nvidia/gemma-4-31b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>`
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
[transformers] Token indices sequence length is longer than the specified maximum sequence length for this model (159385 > 1024). Running this sequence through the model will result in indexing errors
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 11 tokens (Server: 33, Local: 22)
Warmup (System+Empty) complete. Delta: 17 tokens (Server: 39, Local: 22)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.65 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model              |        test |     t/s (total) |       t/s (req) |     peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-------------------|------------:|----------------:|----------------:|-------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| nvidia/gemma-4-31b | pp2048 (c4) | 1813.64 ± 11.61 | 712.09 ± 187.97 |              |                  | 2883.02 ± 853.30 | 2878.38 ± 853.30 | 2883.02 ± 853.30 |
| nvidia/gemma-4-31b |   tg32 (c4) |    18.17 ± 0.13 |     5.36 ± 0.72 | 28.00 ± 0.00 |      7.00 ± 0.00 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 22:43:22 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
