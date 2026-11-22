# Amit Kumar Koshta

**Data & Agentic AI Engineer** · Designing deterministic, observable multi-agent architectures, application-layer AI safety runtimes, and production cloud ML/data pipelines.

[![Email](https://img.shields.io/badge/Email-kenseiamit%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:kenseiamit@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-kenseiAmit-181717?style=flat-square&logo=github)](https://github.com/kenseiAmit)

---

### Featured Engineering Systems

| System | Architectural Focus | Core Stack | Verification |
|:---|:---|:---|:---:|
| **[Guarded SalesOps Agent Runtime](https://github.com/kenseiAmit/guarded-salesops-agent-runtime)** | Defense-in-depth B2B CRM agent runtime enforcing pre/post-inference guardrails, AST-validated Python sandboxing, HITL email approval gates, multi-tenant SQLite state isolation, and recursive PII trace scrubbing. | `Python` · `Anthropic Claude` · `Pydantic` · `AST Sandbox` · `SQLite` · `Docker` | [![CI](https://github.com/kenseiAmit/guarded-salesops-agent-runtime/actions/workflows/ci.yml/badge.svg)](https://github.com/kenseiAmit/guarded-salesops-agent-runtime/actions/workflows/ci.yml) |
| **[Multi-Agent Banking System (A2A + LangGraph)](https://github.com/kenseiAmit/multi-agent-banking-system)** | Decoupled retail banking microservices (`manager`, `deposit`, `loan`) communicating over Agent-to-Agent (A2A) JSON-RPC + MCP SQL Toolbox, paired with a LangGraph intent router and deterministic Python loan underwriting math (`TotalValueAgent`). | `Google ADK` · `A2A Protocol` · `LangGraph` · `MCP` · `Vertex AI` · `MySQL` | [![CI](https://github.com/kenseiAmit/multi-agent-banking-system/actions/workflows/ci.yml/badge.svg)](https://github.com/kenseiAmit/multi-agent-banking-system/actions/workflows/ci.yml) |
| **[Census Income Classification API](https://github.com/kenseiAmit/census-income-api)** | End-to-end MLOps pipeline with leakage-safe preprocessing, automated subgroup fairness auditing across 8 demographic dimensions, Model Card governance, and gated CI/CD cloud deployment on Render. | `FastAPI` · `Scikit-Learn` · `Pandas` · `Pytest` · `GitHub Actions` | [![CI](https://github.com/kenseiAmit/census-income-api/actions/workflows/ci.yml/badge.svg)](https://github.com/kenseiAmit/census-income-api/actions/workflows/ci.yml) |
| **[Abstractive Text Summarization Pipeline](https://github.com/kenseiAmit/Text-Summarizer-Project)** | Config-driven 4-stage NLP training pipeline (ingestion, validation, tokenization, fine-tuning) built on Hugging Face `google/pegasus-cnn_dailymail` and the SAMSum dialogue corpus. | `PyTorch` · `Transformers` · `PEGASUS` · `Hugging Face` · `Docker` | `MIT` |

---

### Core Technical Stack

- **Agentic AI & Orchestration:** Anthropic Claude SDK · LangGraph / LangChain · Google Agent Development Kit (ADK) · Agent-to-Agent (A2A) JSON-RPC · Model Context Protocol (MCP) · Semantic Kernel
- **AI Safety, Eval & AgentOps:** Multi-Tier Runtime Guardrails · AST Code Sandboxing · Human-in-the-Loop (HITL) Gates · Automated Regression Benchmarks · Redacted Structured Telemetry
- **Data Engineering & MLOps:** Python · SQL · Apache Spark · BigQuery · FastAPI · Scikit-Learn · MLflow · Docker · GitHub Actions CI/CD · Cloud Platforms (GCP, AWS, Azure)

---

### Engineering Principles

1. **Deterministic Boundaries Around Probabilistic Models:** Offload arithmetic, policy thresholds, and access control to deterministic Python middleware and custom agents rather than trusting LLM prompts alone.
2. **Zero-Knowledge & Least-Privilege Tooling:** Partition multi-agent capabilities across explicit protocol boundaries (A2A / MCP) so agents exchange verified boolean assertions instead of raw sensitive records.
3. **Observability Without Leakage:** Instrument every agent step for latency, token cost, and guardrail telemetry while scrubbing secrets and restricted PII prior to trace persistence.
