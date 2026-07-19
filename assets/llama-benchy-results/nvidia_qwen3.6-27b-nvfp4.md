(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-27b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:29:11
Benchmarking model: nvidia/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-27b': nvidia/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cfb58-4be7261952e18d70199f8d55;0f4168cc-c443-4f7a-87b1-41be6193ae4e)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-27b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.27 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model              |   test |            t/s |     peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------|-------:|---------------:|-------------:|----------------:|----------------:|----------------:|
| nvidia/qwen3.6-27b | pp2048 | 1041.39 ± 4.56 |              | 1767.81 ± 32.03 | 1764.54 ± 32.03 | 1767.81 ± 32.03 |
| nvidia/qwen3.6-27b |   tg32 |   41.83 ± 0.05 | 43.18 ± 0.06 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:29:11 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-27b" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:29:29
Benchmarking model: nvidia/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-27b': nvidia/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cfb69-7e317e374307d7dd7a399e1f;27f8ad2f-533b-46c5-a330-f08ea1baa502)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-27b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.19 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model              |   test |            t/s |     peak t/s |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------|-------:|---------------:|-------------:|----------------:|----------------:|----------------:|
| nvidia/qwen3.6-27b | pp2048 | 1045.58 ± 0.49 |              | 1775.75 ± 33.08 | 1772.56 ± 33.08 | 1775.75 ± 33.08 |
| nvidia/qwen3.6-27b |   tg32 |   51.94 ± 8.86 | 53.61 ± 9.15 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:29:29 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-27b" --concurrency=2
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:30:55
Benchmarking model: nvidia/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [2]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-27b': nvidia/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cfbbf-5355b9a4729447e7008b7314;d6752be3-b772-458a-9554-96589b3c5ef3)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-27b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.15 ms
Running test: pp=2048, tg=32, depth=0, concurrency=2
  Warmup 1/1 (batch size 2)...
  Run 1/3 (batch size 2)...
  Run 2/3 (batch size 2)...
  Run 3/3 (batch size 2)...
Printing results in MD format:



| model              |        test |    t/s (total) |      t/s (req) |     peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------|------------:|---------------:|---------------:|-------------:|-----------------:|----------------:|----------------:|----------------:|
| nvidia/qwen3.6-27b | pp2048 (c2) | 1049.31 ± 4.90 | 536.27 ± 13.24 |              |                  | 3390.20 ± 76.39 | 3387.06 ± 76.39 | 3390.20 ± 76.39 |
| nvidia/qwen3.6-27b |   tg32 (c2) |   71.91 ± 5.90 |   44.26 ± 6.55 | 74.23 ± 6.09 |     45.69 ± 6.76 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:30:55 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-27b" --concurrency=2
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:33:24
Benchmarking model: nvidia/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [2]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-27b': nvidia/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cfc54-10c407cd53eb86a51a86426d;8415858f-357c-4798-81ef-72425d9375eb)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-27b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.30 ms
Running test: pp=2048, tg=32, depth=0, concurrency=2
  Warmup 1/1 (batch size 2)...
  Run 1/3 (batch size 2)...
  Run 2/3 (batch size 2)...
  Run 3/3 (batch size 2)...
Printing results in MD format:



| model              |        test |    t/s (total) |     t/s (req) |     peak t/s |   peak t/s (req) |       ttfr (ms) |    est_ppt (ms) |   e2e_ttft (ms) |
|:-------------------|------------:|---------------:|--------------:|-------------:|-----------------:|----------------:|----------------:|----------------:|
| nvidia/qwen3.6-27b | pp2048 (c2) | 1062.16 ± 4.06 | 542.42 ± 5.00 |              |                  | 3468.59 ± 83.49 | 3465.30 ± 83.49 | 3468.59 ± 83.49 |
| nvidia/qwen3.6-27b |   tg32 (c2) |   61.89 ± 2.36 |  36.08 ± 4.50 | 64.74 ± 1.24 |     37.24 ± 4.65 |                 |                 |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:33:24 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-27b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:44:13
Benchmarking model: nvidia/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-27b': nvidia/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5cfedd-0e3aace403a393e72469e21c;1a5155a8-5aad-422b-912e-74fce2f36354)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-27b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup failed: HTTP 500: {"error":{"message":"litellm.InternalServerError: InternalServerError: OpenAIException - Connection error.. Received Model Group=nvidia/qwen3.6-27b\nAvailable Model Group Fallbacks=None","type":null,"param":null,"code":"500"}}
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-27b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:50:12
Benchmarking model: nvidia/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-27b': nvidia/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d0044-662b44fc477a6c5564dbdecc;21fec647-245a-4a8b-ba19-5cb708e45f62)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-27b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.61 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model              |        test |    t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-------------------|------------:|---------------:|---------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| nvidia/qwen3.6-27b | pp2048 (c4) | 1077.68 ± 2.90 | 286.77 ± 22.71 |               |                  | 6454.34 ± 479.66 | 6450.73 ± 479.66 | 6454.34 ± 479.66 |
| nvidia/qwen3.6-27b |   tg32 (c4) |   57.12 ± 4.56 |   29.07 ± 8.04 | 110.67 ± 6.02 |     31.84 ± 6.72 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:50:12 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "nvidia/qwen3.6-27b" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 18:51:21
Benchmarking model: nvidia/qwen3.6-27b at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'nvidia/qwen3.6-27b': nvidia/qwen3.6-27b is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d0089-4661d30b38ab528d01463398;2827bf72-73d4-457a-9831-9facc3ebdc47)

Repository Not Found for url: https://huggingface.co/nvidia/qwen3.6-27b/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 8 tokens (Server: 30, Local: 22)
Warmup (System+Probe) complete. Delta: 13 tokens (Server: 36, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.19 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model              |        test |    t/s (total) |      t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:-------------------|------------:|---------------:|---------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| nvidia/qwen3.6-27b | pp2048 (c4) | 1083.58 ± 1.42 | 289.56 ± 21.99 |               |                  | 6548.97 ± 509.27 | 6545.78 ± 509.27 | 6548.97 ± 509.27 |
| nvidia/qwen3.6-27b |   tg32 (c4) |   57.06 ± 2.44 |   29.91 ± 8.80 | 108.67 ± 2.36 |     31.92 ± 7.55 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 18:51:21 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
