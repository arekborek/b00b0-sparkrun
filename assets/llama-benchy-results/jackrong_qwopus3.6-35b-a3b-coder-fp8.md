(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwopus3.6-35b-coder" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 20:08:29
Benchmarking model: qwopus3.6-35b-coder at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwopus3.6-35b-coder': qwopus3.6-35b-coder is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d129d-1b8df4c84350b5187c42a500;d200c4c0-3134-4931-ac41-d274713579dd)

Repository Not Found for url: https://huggingface.co/qwopus3.6-35b-coder/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.48 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model               |   test |              t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------|-------:|-----------------:|-------------:|---------------:|---------------:|----------------:|
| qwopus3.6-35b-coder | pp2048 | 3853.43 ± 454.72 |              | 497.64 ± 68.80 | 493.16 ± 68.80 |  497.64 ± 68.80 |
| qwopus3.6-35b-coder |   tg32 |     51.32 ± 0.43 | 52.98 ± 0.44 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 20:08:29 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwopus3.6-35b-coder" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 20:08:38
Benchmarking model: qwopus3.6-35b-coder at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwopus3.6-35b-coder': qwopus3.6-35b-coder is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d12a6-50cd9dd65d1a96e443c77fad;032842a9-aa39-469f-b388-e2d7767761fc)

Repository Not Found for url: https://huggingface.co/qwopus3.6-35b-coder/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.83 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model               |   test |             t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:--------------------|-------:|----------------:|-------------:|---------------:|---------------:|----------------:|
| qwopus3.6-35b-coder | pp2048 | 4122.03 ± 91.02 |              | 443.83 ± 16.10 | 439.00 ± 16.10 |  443.83 ± 16.10 |
| qwopus3.6-35b-coder |   tg32 |    51.62 ± 0.16 | 53.28 ± 0.17 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 20:08:38 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwopus3.6-35b-coder" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 20:08:48
Benchmarking model: qwopus3.6-35b-coder at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwopus3.6-35b-coder': qwopus3.6-35b-coder is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d12b0-7318c23d05ac2cbf624ecae0;c577100f-c1a2-49ab-ba82-3253e2fa38fa)

Repository Not Found for url: https://huggingface.co/qwopus3.6-35b-coder/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 4.47 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model               |        test |      t/s (total) |        t/s (req) |       peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:--------------------|------------:|-----------------:|-----------------:|---------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| qwopus3.6-35b-coder | pp2048 (c4) | 4424.48 ± 658.67 | 1277.45 ± 332.01 |                |                  | 1563.53 ± 348.32 | 1559.06 ± 348.32 | 1563.53 ± 348.32 |
| qwopus3.6-35b-coder |   tg32 (c4) |     68.68 ± 2.48 |     27.69 ± 5.20 | 115.33 ± 12.26 |     31.23 ± 1.72 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 20:08:48 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "qwopus3.6-35b-coder" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 20:12:06
Benchmarking model: qwopus3.6-35b-coder at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'qwopus3.6-35b-coder': qwopus3.6-35b-coder is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d1376-1a7a184b78c32b10301d931a;580045bd-be49-4059-8a56-d63fbf12ca54)

Repository Not Found for url: https://huggingface.co/qwopus3.6-35b-coder/resolve/main/tokenizer.json.
Please make sure you specified the correct `repo_id` and `repo_type`.
If you are trying to access a private or gated repo, make sure you are authenticated and your token has the required permissions.
For more details, see https://huggingface.co/docs/huggingface_hub/authentication
Invalid username or password.)
Falling back to 'gpt2' tokenizer as approximation.
Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
Loading text from cache: /Users/arek/.cache/llama-benchy/cc6a0b5782734ee3b9069aa3b64cc62c.txt
Total tokens available in text corpus: 159385
Warming up...
Warmup (User only) complete. Delta: 10 tokens (Server: 32, Local: 22)
Warmup (System+Probe) complete. Delta: 15 tokens (Server: 38, Local context: 22, Probe: 1)

Running coherence test...
Coherence test PASSED.
Measuring latency using mode: api...
Average latency (api): 3.34 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model               |        test |      t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:--------------------|------------:|-----------------:|-----------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| qwopus3.6-35b-coder | pp2048 (c4) | 4922.86 ± 657.07 | 1416.00 ± 369.15 |               |                  | 1384.07 ± 324.38 | 1380.74 ± 324.38 | 1384.07 ± 324.38 |
| qwopus3.6-35b-coder |   tg32 (c4) |     77.76 ± 4.67 |     27.50 ± 4.46 | 121.33 ± 1.89 |     30.33 ± 0.47 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 20:12:06 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
