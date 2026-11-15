<a href="https://github.com/pavan139">
  <img src="./assets/header.svg" width="100%" alt="Pavan Reddy Mogili, Applied AI Engineer. Open to Applied AI and LLM platform roles. I build the reliability layer around LLMs: retrieval, evaluation, agent safety and inference.">
</a>

<p align="center">
  <a href="https://www.linkedin.com/in/pavan-reddy-mogili/"><img src="./assets/btn-linkedin.svg" height="46" alt="Connect with Pavan Reddy Mogili on LinkedIn"></a>&nbsp;
  <a href="mailto:pavanreddy139@gmail.com"><img src="./assets/btn-email.svg" height="46" alt="Email Pavan Reddy Mogili"></a>&nbsp;
  <a href="#selected-work"><img src="./assets/btn-work.svg" height="46" alt="Jump to Pavan's selected AI engineering projects"></a>
</p>

## Hi, I'm Pavan 👋

I'm an **Applied AI Engineer** who likes the unglamorous half of AI: the retrieval layer that decides what a model gets to see, the eval that catches a regression before a user does, the permission check in front of every tool call, and the runtime that survives a crash at the worst possible moment.

I came to this from the data side. I'm currently at **Fidelity Investments**, and before that I worked on biomedical **NLP** at **Affinia Therapeutics** and data engineering at **Cognizant**. Real data and real users taught me that the model is rarely the part that breaks. Everything around it is.

- 🔭 **Focus:** LLM applications, retrieval-augmented generation (RAG), LLM evaluation, AI agent platforms, reliable inference
- 🧑‍💻 **Languages:** Python every day, plus Go, Swift, SQL and TypeScript
- 🎓 **Education:** M.S. in Data Science, Northeastern University · doctoral student, University of the Cumberlands
- 📱 **Building:** Turtledove, an iPhone app for couples (closed beta)
- 💼 **Open to:** Applied AI, LLM platform and ML infrastructure roles

## 🕊️ Building now: Turtledove

<img src="./assets/turtledove.svg" width="100%" alt="Turtledove, a SwiftUI iPhone app for couples built by Pavan Reddy Mogili: shared plans, trips, habits and a journal, with widgets, Siri, on-device Apple Intelligence, a Supabase Postgres backend and an MCP server for AI assistants. Closed beta on TestFlight.">

Turtledove is a shared-life app for couples: plans, trips, habits you keep together and a shared journal, in one place for two. I'm designing and building it solo, end to end.

- **iOS:** native SwiftUI with SwiftData, WidgetKit widgets, App Intents for Siri and Shortcuts, and on-device Apple Intelligence for search and spelling, so nothing personal leaves the phone
- **Backend:** Supabase with Postgres row-level security, transactional pairing, Deno edge functions and a push notification worker
- **AI integration:** a remote MCP server (32 tools, OAuth 2.1) so assistants like ChatGPT and Claude can read and add plans, with every connection approved on your iPhone
- **Status:** closed beta on TestFlight. The code is private for now, and I'm happy to walk through it in an interview.

<a id="selected-work"></a>

## 🧪 Selected work

Each project starts from a failure mode that bites real AI systems, and ships with code, tests and an honest write-up of what the experiments show (and what they don't).

<p>
  <a href="https://github.com/pavan139/resilient-agent-runtime"><img src="./assets/cards/resilient-agent-runtime.svg" width="49%" alt="Resilient Agent Runtime (Python): transactional outbox and inbox, payload-bound deduplication and crash recovery so AI agent side effects run exactly once."></a>
  <a href="https://github.com/pavan139/capability-guard"><img src="./assets/cards/capability-guard.svg" width="49%" alt="Capability Guard (Python): HMAC-signed least-privilege capabilities for LLM tool use with scopes, revocation, quotas and replay protection."></a>
  <a href="https://github.com/pavan139/tool-calling-lab"><img src="./assets/cards/tool-calling-lab.svg" width="49%" alt="Tool Calling Lab (Python): execution-based evaluation of LLM tool calls, synthetic data, LoRA supervised fine-tuning and DPO preference optimization."></a>
  <a href="https://github.com/pavan139/agent-regression"><img src="./assets/cards/agent-regression.svg" width="49%" alt="Agent Regression (Python): regression testing for AI agents that grades outputs and execution traces against independent oracles to gate releases."></a>
  <a href="https://github.com/pavan139/temporal-rag"><img src="./assets/cards/temporal-rag.svg" width="49%" alt="Temporal RAG (Python): retrieval-augmented generation over changing facts with bitemporal queries, provenance, citations and abstention."></a>
  <a href="https://github.com/pavan139/hard-negative-retrieval"><img src="./assets/cards/hard-negative-retrieval.svg" width="49%" alt="Hard-Negative Retrieval (Python): contrastive embedding training with hard-negative mining, late-interaction MaxSim scoring and approximate nearest neighbor index evaluation."></a>
  <a href="https://github.com/pavan139/speculative-decoding"><img src="./assets/cards/speculative-decoding.svg" width="49%" alt="Speculative Decoding (Python): exact draft-and-verify rejection sampling for faster LLM inference with KV-cache recovery and profiling."></a>
  <a href="https://github.com/pavan139/servegate"><img src="./assets/cards/servegate.svg" width="49%" alt="ServeGate (Go): model serving gateway with deadline-aware microbatching, fair multi-tenant admission control, cancellation and circuit breaking."></a>
</p>

### More from the lab

| Area | Project | What it explores |
| --- | --- | --- |
| LLM systems | [model-router](https://github.com/pavan139/model-router) | Learned routing between cheaper and stronger models under a budget, with held-out evaluation and calibration |
| LLM systems | [constrained-generation](https://github.com/pavan139/constrained-generation) | Grammar-constrained decoding with incremental parsing, token masks and bounded interpreters |
| Agents | [agent-arena](https://github.com/pavan139/agent-arena) | D* Lite incremental replanning for bounded agents with typed tools |
| Vision + ML | [pixel-to-program](https://github.com/pavan139/pixel-to-program) | An encoder-decoder that reads an image and writes the program that draws it |
| MLOps | [drift-sentinel](https://github.com/pavan139/drift-sentinel) | Sequential drift monitoring with delayed labels and a real alert lifecycle |
| MLOps | [model-ledger](https://github.com/pavan139/model-ledger) | Content-addressed model registry with lineage, compare-and-swap promotions and rollback |
| MLOps | [chronofeature](https://github.com/pavan139/chronofeature) | Point-in-time feature store that keeps future data out of training, with offline/online parity |
| Data systems | [eventflow](https://github.com/pavan139/eventflow) | Event-time stream processing: watermarks, retractions, checkpoints and deterministic recovery |
| Data systems | [incremental-lakehouse](https://github.com/pavan139/incremental-lakehouse) | Incremental CDC warehouse with schema contracts, lineage and atomic publish |
| Data systems | [query-forge](https://github.com/pavan139/query-forge) | A small SQL engine: parser, relational plans and join optimization, checked against SQLite |
| Distributed systems | [quorum-lab](https://github.com/pavan139/quorum-lab) | Durable Raft in Go under network partitions and restarts, with a safety checker |

## 🧭 How I think about AI systems

| When I look at... | ...I want to know |
| --- | --- |
| **Retrieval** | Is the evidence relevant, permitted, current and sufficient? Can the system say "I don't know"? |
| **Evaluation** | What is the independent oracle? Which cases fail? Would the release gate have caught last month's regression? |
| **Agent safety** | Who authorizes a tool's side effects? Can a request exceed its scope or replay a committed action? |
| **Reliability** | What happens after a timeout, a duplicate delivery, a stale lease or a crash between two commits? |
| **Performance** | What workload was measured, and what does the latency or cost number actually include? |

## 🧰 Toolbox

<img src="./assets/toolbox.svg" width="100%" alt="Toolbox. AI and LLM: PyTorch, Hugging Face, RAG, embeddings, LoRA, SFT, DPO, LLM evals, tool calling, MCP, on-device AI. Backend and data: Python, Go, FastAPI, Pydantic, TypeScript, SQL, PostgreSQL, SQLite, pandas, Snowflake, Supabase. Infra and apps: Docker, Kubernetes, AWS, GitHub Actions, CI/CD, observability, Swift, SwiftUI, Deno.">

## 🌱 Off the keyboard

- 📚 Doctoral student at the University of the Cumberlands. My research interest: how LLMs actually change everyday work.
- 🏔️ Happiest on a road trip with a national park at the end of it.
- 🏃 Slowly, stubbornly training for a 5K.
- ✍️ I write READMEs the way I like to read them: what broke, what I tried, and what the numbers actually say.

<a href="mailto:pavanreddy139@gmail.com">
  <img src="./assets/footer.svg" width="100%" alt="Thanks for stopping by. Building something with LLMs that has to actually work? Email pavanreddy139@gmail.com or connect with Pavan Reddy Mogili on LinkedIn.">
</a>
