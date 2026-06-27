(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:01:38
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.48 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |              t/s |      peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|-----------------:|--------------:|---------------:|---------------:|----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 | 2832.70 ± 197.17 |               | 662.06 ± 63.20 | 658.58 ± 63.20 |  662.06 ± 63.20 |
| nvidia/qwen3.6-35b-a3b |   tg32 |    107.34 ± 6.78 | 110.87 ± 7.00 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:01:38 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=1
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:01:51
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
Error loading tokenizer: nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 4.40 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                  |   test |              t/s |      peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:-----------------------|-------:|-----------------:|--------------:|---------------:|---------------:|----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 | 2813.60 ± 201.07 |               | 664.10 ± 67.45 | 659.70 ± 67.45 |  664.10 ± 67.45 |
| nvidia/qwen3.6-35b-a3b |   tg32 |    108.92 ± 7.06 | 112.48 ± 7.29 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:01:51 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:02:02
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 3.29 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |      t/s (total) |        t/s (req) |       peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-----------------------|------------:|-----------------:|-----------------:|---------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 (c4) | 5504.17 ± 894.33 | 1405.56 ± 240.51 |                |                  | 1371.33 ± 247.75 | 1368.04 ± 247.75 | 1371.33 ± 247.75 |
| nvidia/qwen3.6-35b-a3b |   tg32 (c4) |   244.40 ± 18.52 |     72.55 ± 6.84 | 252.28 ± 19.12 |     74.92 ± 7.06 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:02:02 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-35b-a3b" --concurrency=4
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-06-06 15:02:20
Benchmarking model: nvidia/qwen3.6-35b-a3b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
Error loading tokenizer: nvidia/qwen3.6-35b-a3b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
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
Average latency (api): 2.09 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                  |        test |      t/s (total) |        t/s (req) |       peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-----------------------|------------:|-----------------:|-----------------:|---------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| nvidia/qwen3.6-35b-a3b | pp2048 (c4) | 5706.29 ± 673.07 | 1461.51 ± 177.22 |                |                  | 1295.84 ± 187.40 | 1293.75 ± 187.40 | 1295.84 ± 187.40 |
| nvidia/qwen3.6-35b-a3b |   tg32 (c4) |   270.55 ± 18.03 |     73.24 ± 7.74 | 279.28 ± 18.61 |     75.63 ± 8.00 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-06-06 15:02:20 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
