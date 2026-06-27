(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/gemma-4-26b-a4b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 21:40:38
Benchmarking model: nvidia/gemma-4-26b-a4b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: nvidia/gemma-4-26b-a4b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.49 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |             t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|----------------:|-------------:|---------------:|---------------:|----------------:|
| nvidia/gemma-4-26b-a4b | pp2048 | 5993.11 ± 45.28 |              | 307.23 ± 10.23 | 303.74 ± 10.23 |  307.23 ± 10.23 |
| nvidia/gemma-4-26b-a4b |   tg32 |    30.04 ± 0.03 | 31.00 ± 0.00 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 21:40:38 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/gemma-4-26b-a4b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 21:40:53
Benchmarking model: nvidia/gemma-4-26b-a4b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: nvidia/gemma-4-26b-a4b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 2.49 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |             t/s |     peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|----------------:|-------------:|--------------:|---------------:|----------------:|
| nvidia/gemma-4-26b-a4b | pp2048 | 5996.02 ± 33.08 |              | 305.74 ± 4.23 |  303.25 ± 4.23 |   305.74 ± 4.23 |
| nvidia/gemma-4-26b-a4b |   tg32 |    30.01 ± 0.04 | 31.00 ± 0.00 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 21:40:53 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/gemma-4-26b-a4b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 21:41:04
Benchmarking model: nvidia/gemma-4-26b-a4b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: nvidia/gemma-4-26b-a4b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.04 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |      t/s (total) |         t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|------------:|-----------------:|------------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| nvidia/gemma-4-26b-a4b | pp2048 (c4) | 6339.54 ± 158.96 | 2378.51 ± 1025.72 |               |                  | 909.56 ± 312.82 | 906.52 ± 312.82 | 909.56 ± 312.82 |
| nvidia/gemma-4-26b-a4b |   tg32 (c4) |     71.84 ± 5.21 |      24.47 ± 4.70 | 116.00 ± 3.27 |     29.00 ± 0.82 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 21:41:04 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/gemma-4-26b-a4b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 21:41:22
Benchmarking model: nvidia/gemma-4-26b-a4b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: nvidia/gemma-4-26b-a4b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.92 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |     t/s (total) |         t/s (req) |      peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|------------:|----------------:|------------------:|--------------:|-----------------:|----------------:|----------------:|----------------:|
| nvidia/gemma-4-26b-a4b | pp2048 (c4) | 6593.48 ± 91.00 | 2545.27 ± 1238.65 |               |                  | 868.55 ± 304.39 | 864.63 ± 304.39 | 868.55 ± 304.39 |
| nvidia/gemma-4-26b-a4b |   tg32 (c4) |    70.53 ± 4.25 |      23.71 ± 4.48 | 112.00 ± 0.00 |     28.00 ± 0.00 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 21:41:22 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
