(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "empero-ai/qwythos-9b-mythos" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 19:10:03
Benchmarking model: empero-ai/qwythos-9b-mythos at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'empero-ai/qwythos-9b-mythos': empero-ai/qwythos-9b-mythos is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d04eb-681e561a56bcb5f56155dc39;c154963f-593c-43c7-baea-e39055f0d8d2)

Repository Not Found for url: https://huggingface.co/empero-ai/qwythos-9b-mythos/resolve/main/tokenizer.json.
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
Average latency (api): 2.96 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                       |   test |            t/s |     peak t/s |      ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:----------------------------|-------:|---------------:|-------------:|---------------:|---------------:|----------------:|
| empero-ai/qwythos-9b-mythos | pp2048 | 3361.49 ± 7.62 |              | 548.12 ± 15.27 | 545.16 ± 15.27 |  548.12 ± 15.27 |
| empero-ai/qwythos-9b-mythos |   tg32 |   23.77 ± 0.03 | 24.00 ± 0.00 |                |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 19:10:03 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "empero-ai/qwythos-9b-mythos" --concurrency=1
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 19:10:21
Benchmarking model: empero-ai/qwythos-9b-mythos at http://gx10-d2cf.local:4000/v1
Concurrency levels: [1]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'empero-ai/qwythos-9b-mythos': empero-ai/qwythos-9b-mythos is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d04fd-6242c5dd7f4162067c99fcd9;ed1bf4b3-4306-46bf-931f-eac1585de271)

Repository Not Found for url: https://huggingface.co/empero-ai/qwythos-9b-mythos/resolve/main/tokenizer.json.
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
Average latency (api): 2.56 ms
Running test: pp=2048, tg=32, depth=0, concurrency=1
  Warmup 1/1 (batch size 1)...
  Run 1/3 (batch size 1)...
  Run 2/3 (batch size 1)...
  Run 3/3 (batch size 1)...
Printing results in MD format:



| model                       |   test |             t/s |     peak t/s |     ttfr (ms) |   est_ppt (ms) |   e2e_ttft (ms) |
|:----------------------------|-------:|----------------:|-------------:|--------------:|---------------:|----------------:|
| empero-ai/qwythos-9b-mythos | pp2048 | 3372.13 ± 14.57 |              | 549.10 ± 7.81 |  546.55 ± 7.81 |   549.10 ± 7.81 |
| empero-ai/qwythos-9b-mythos |   tg32 |    23.84 ± 0.01 | 24.00 ± 0.00 |               |                |                 |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 19:10:21 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "empero-ai/qwythos-9b-mythos" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 19:10:40
Benchmarking model: empero-ai/qwythos-9b-mythos at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'empero-ai/qwythos-9b-mythos': empero-ai/qwythos-9b-mythos is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d0510-04ebc12e2f011a5a77de4ff4;3dd1f870-ae8d-4234-a4ff-431c458ef885)

Repository Not Found for url: https://huggingface.co/empero-ai/qwythos-9b-mythos/resolve/main/tokenizer.json.
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
Average latency (api): 2.36 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                       |        test |    t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:----------------------------|------------:|---------------:|-----------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| empero-ai/qwythos-9b-mythos | pp2048 (c4) | 3518.06 ± 2.74 | 1264.14 ± 652.65 |               |                  | 1782.12 ± 588.83 | 1779.76 ± 588.83 | 1782.12 ± 588.83 |
| empero-ai/qwythos-9b-mythos |   tg32 (c4) |   49.32 ± 0.34 |     23.24 ± 6.18 | 109.00 ± 1.41 |     27.25 ± 0.43 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 19:10:40 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % llama-benchy --base-url "http://gx10-d2cf.local:4000/v1" --model "empero-ai/qwythos-9b-mythos" --concurrency=4
llama-benchy (0.3.8.dev2+gff162bcfc)
Date: 2026-07-19 19:11:05
Benchmarking model: empero-ai/qwythos-9b-mythos at http://gx10-d2cf.local:4000/v1
Concurrency levels: [4]
[transformers] PyTorch was not found. Models won't be available and only tokenizers, configuration and file/data utilities can be used.
Error loading tokenizer 'empero-ai/qwythos-9b-mythos': empero-ai/qwythos-9b-mythos is not a local folder and is not a valid model identifier listed on 'https://huggingface.co/models'
If this is a private repository, make sure to pass a token having permission to this repo either by logging in with `hf auth login` or by passing `token=<your_token>` (lightweight tokenizer error: 401 Client Error. (Request ID: Root=1-6a5d0529-65e24eab5a82811102432ece;74c53a17-72e6-4591-8832-30d646132b1f)

Repository Not Found for url: https://huggingface.co/empero-ai/qwythos-9b-mythos/resolve/main/tokenizer.json.
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
Average latency (api): 2.80 ms
Running test: pp=2048, tg=32, depth=0, concurrency=4
  Warmup 1/1 (batch size 4)...
  Run 1/3 (batch size 4)...
  Run 2/3 (batch size 4)...
  Run 3/3 (batch size 4)...
Printing results in MD format:



| model                       |        test |     t/s (total) |        t/s (req) |      peak t/s |   peak t/s (req) |        ttfr (ms) |     est_ppt (ms) |    e2e_ttft (ms) |
|:----------------------------|------------:|----------------:|-----------------:|--------------:|-----------------:|-----------------:|-----------------:|-----------------:|
| empero-ai/qwythos-9b-mythos | pp2048 (c4) | 3520.87 ± 11.14 | 1272.46 ± 676.65 |               |                  | 1774.70 ± 585.10 | 1771.90 ± 585.10 | 1774.70 ± 585.10 |
| empero-ai/qwythos-9b-mythos |   tg32 (c4) |    49.51 ± 0.43 |     23.28 ± 6.19 | 108.00 ± 0.00 |     27.00 ± 0.00 |                  |                  |                  |

llama-benchy (0.3.8.dev2+gff162bcfc)
date: 2026-07-19 19:11:05 | latency mode: api
(llama-benchy) arek@DESKTOP-15MQGOE llama-benchy % 
