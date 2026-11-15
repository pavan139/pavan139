# Pavan Reddy Mogili

**Applied AI Engineer** · Retrieval & RAG · Evaluation · Agent Systems · Inference Engineering

I build software around AI models: the retrieval layer that supplies evidence, the evaluation harness that catches regressions, the tool boundary that limits actions, and the runtime that survives partial failure.

My background spans enterprise software and data engineering, applied machine learning, and customer-facing delivery. I currently work at **Fidelity Investments**. Previously: biomedical NLP at **Affinia Therapeutics** and backend engineering at **Cognizant**.

[LinkedIn](https://www.linkedin.com/in/pavan-reddy-mogili/) · [Email](mailto:pavanreddy139@gmail.com) · [Repositories](https://github.com/pavan139?tab=repositories)

---

## Selected work

These are public, reproducible projects. Each one starts with an engineering failure mode and includes code, checks, and a record of what the experiments actually establish.

### 01. Agent execution and safety

**[Resilient Agent Runtime](https://github.com/pavan139/resilient-agent-runtime)**  
*Transactional outbox/inbox · Idempotency · Crash recovery*

The receiver commits an effect, but the sender crashes before acknowledging it. A two-database SQLite implementation explores how to redeliver safely using payload-bound inbox identities, fenced dispatch claims, and durable workflow state. The result distinguishes delivery acknowledgments from actual receiver effects.

[Implementation](https://github.com/pavan139/resilient-agent-runtime/tree/project-main/src) · [Recovery tests](https://github.com/pavan139/resilient-agent-runtime/tree/project-main/verification) · [Recorded replay](https://github.com/pavan139/resilient-agent-runtime/blob/project-main/replays/outbox-demo.json)

**[Capability Guard](https://github.com/pavan139/capability-guard)**  
*Least-privilege tool use · Authorization · Replay protection*

An agent should not be able to grant itself permissions through text. This project issues host-controlled HMAC capabilities and checks scope, revocation, quotas, ancestry, and fresh nonces before local effects. Quota usage and effect commit atomically in SQLite.

[Threat model](https://github.com/pavan139/capability-guard/tree/project-main/security) · [Adversarial checks](https://github.com/pavan139/capability-guard/tree/project-main/adversarial)

### 02. Model behavior and evaluation

**[Tool Calling Lab](https://github.com/pavan139/tool-calling-lab)**  
*Structured tool programs · Execution-based evaluation · SFT / DPO*

A syntactically valid tool call can still fail the task. This lab scores structured programs against an independent stateful executor, generates preference pairs from execution results, and includes optional LoRA SFT and DPO experiments. Its deterministic reference baseline is not presented as model accuracy.

[Executor contract](https://github.com/pavan139/tool-calling-lab/blob/project-main/notes/robot-execution.md) · [Training methodology](https://github.com/pavan139/tool-calling-lab/blob/project-main/notes/preference-optimization.md)

**[Speculative Decoding](https://github.com/pavan139/speculative-decoding)**  
*Inference algorithms · Probability correctness · KV-cache behavior*

Implements draft/target rejection sampling and cached block verification. Tests probability distributions against an enumerated reference and checks cache recovery after rejected tokens. CPU timing results are explicitly scoped to tiny locally generated checkpoints.

[Correctness notebook](https://github.com/pavan139/speculative-decoding/blob/project-main/research/correctness-notebook.md) · [Measurement protocol](https://github.com/pavan139/speculative-decoding/blob/project-main/research/measurement-protocol.md)

### 03. Monitoring and data reliability

**[Drift Sentinel](https://github.com/pavan139/drift-sentinel)**  
*Sequential monitoring · Delayed labels · Alert lifecycle*

Separates changes in incoming features from changes in observed prediction quality. Handles delayed labels, deduplicates request identities, and documents the assumptions behind sequential alert thresholds rather than claiming certainty from a small quiet experiment.

[Evaluation](https://github.com/pavan139/drift-sentinel/blob/project-main/measurements/evaluation.json) · [Statistical assumptions](https://github.com/pavan139/drift-sentinel/blob/project-main/analysis/spending-and-delay.md)

**[Eventflow](https://github.com/pavan139/eventflow)**  
*Event-time processing · Late data · Deterministic replay*

Explores what happens when an event arrives after its window has already been published. Implements watermarks, retractions, checkpointing, source deduplication, and replay checks around an atomic SQLite state boundary.

[Eventflow repository](https://github.com/pavan139/eventflow) · [Recovery tests](https://github.com/pavan139/eventflow/tree/project-main/recovery_tests)

Also: **[Incremental Lakehouse](https://github.com/pavan139/incremental-lakehouse)**, a CDC pipeline with schema contracts, atomic publication, and independent rebuild comparisons.

---

## What I optimize for

| Concern | Questions I want answered |
| --- | --- |
| **Retrieval** | Is the evidence relevant, permitted, current, and sufficient to answer? |
| **Evaluation** | What is the independent oracle? Which cases fail? Does the release gate catch regressions? |
| **Agent safety** | Who authorizes tool effects? Can a request exceed its scope or replay a committed action? |
| **Reliability** | What happens after a timeout, duplicate delivery, stale lease, or crash between two commits? |
| **Performance** | What workload was measured? What does latency or cost actually include? |

## Working stack

**AI & evaluation:** RAG, retrieval metrics, embeddings, PyTorch, Hugging Face, structured tool calls, SFT, regression testing  
**Backend & data:** Python, FastAPI, Pydantic, TypeScript, SQL, PostgreSQL, SQLite, pandas, Snowpark  
**Infrastructure:** Docker, Kubernetes, AWS, CI/CD, tracing, observability

---

I am interested in **Applied AI Engineering** roles focused on LLM applications, retrieval, evaluations, agent platforms, and reliable inference systems.

**[Connect on LinkedIn](https://www.linkedin.com/in/pavan-reddy-mogili/)** · **[Email me](mailto:pavanreddy139@gmail.com)**
