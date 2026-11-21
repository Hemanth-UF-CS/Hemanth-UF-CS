### ML systems

| Project | What it is | Built with |
|---|---|---|
| [nanoserve](https://github.com/Hemanth-UF-CS/nanoserve) | A GPT trained from scratch and the platform that serves it: KV cache, continuous batching, CUDA-graph decode, multi-LoRA routing, DPO, int8, and a gateway with failover and per-tenant cost tracking. 61.6k tokens/s on an RTX 4090. Killing a GPU server under load dropped 0 of 38,412 requests. | PyTorch, CUDA, FastAPI, Prometheus |
| [gpu-kernels-dl](https://github.com/Hemanth-UF-CS/gpu-kernels-dl) | Matmul, softmax and reduction kernels written in Triton and CUDA C++, checked against PyTorch and benchmarked with CUDA events. The README explains where cuBLAS stays ahead and why. | Triton, CUDA C++ |
| [llm-inference-runtime](https://github.com/Hemanth-UF-CS/llm-inference-runtime) | An inference runtime for Hugging Face models with a request scheduler, KV-cache pool and asyncio continuous batching. | Python, PyTorch, FastAPI |

### Backend and distributed systems

| Project | What it is | Built with |
|---|---|---|
| [feed-engine](https://github.com/Hemanth-UF-CS/feed-engine) | A social feed backend. Posts fan out through Kafka to per-user Redis sorted sets, consumers are idempotent so events can be replayed safely, and Postgres is the source of truth. | Go, Kafka, Redis, PostgreSQL |
| [Quick_Chat](https://github.com/Hemanth-UF-CS/Quick_Chat) | Real-time chat that scales across server instances using Redis Pub/Sub, with message history served from cache. | Go, WebSockets, Redis, React |
| [File-Transfer-System](https://github.com/Hemanth-UF-CS/File-Transfer-System) | Concurrent upload and download over TCP, one thread per client, with chunked I/O and path sanitisation. | C++17, sockets |
| [BANKING-SYSTEMS](https://github.com/Hemanth-UF-CS/BANKING-SYSTEMS) | A multithreaded banking server with mutex-protected accounts and file-backed persistence. | C++17, sockets |

### AI agents and developer tools

| Project | What it is | Built with |
|---|---|---|
| [VoiceCoder](https://github.com/Hemanth-UF-CS/VoiceCoder) | Voice-driven coding for VS Code. It turns speech into intents (write, refactor, test, commit) and applies reviewable diffs. A local grammar resolves 57% of the eval commands without a model call. | TypeScript, VS Code API, LLMs |
| [multi-agent-orchestrator](https://github.com/Hemanth-UF-CS/multi-agent-orchestrator) | A planner that delegates to retriever, executor and verifier agents over shared typed state, with per-agent tracing and token accounting. | Python, LangGraph |
| [react-agent](https://github.com/Hemanth-UF-CS/react-agent) | A ReAct loop written without a framework: validated tool calls, retry on bad arguments, a self-critique step, and a 30-task eval. | Python, Pydantic |
| [inbox-triage](https://github.com/Hemanth-UF-CS/inbox-triage) | Sorts a shared inbox and drafts replies for a person to review. It never sends mail, and the Gmail permission scope enforces that. | Python, Claude API, Gmail API |

### Apps

| Project | What it is | Built with |
|---|---|---|
| [daily-intake-tracker](https://github.com/Hemanth-UF-CS/daily-intake-tracker) | A nutrition tracker that compares what you ate to daily limits. [Live](https://daily-intake-tracker.vercel.app) | React, TypeScript, Postgres |
| [hustler-console](https://github.com/Hemanth-UF-CS/hustler-console) | A study and job-search planner that works offline as a PWA, or multi-user with Supabase auth and row-level security. | React, TypeScript, Supabase |
