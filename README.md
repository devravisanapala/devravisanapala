# Ravi Sanapala

### AI Engineer · Agentic Systems · Enterprise AI Delivery

I build AI applications that connect language models, business workflows, and the people who use them. My work spans agent orchestration, document intelligence, full-stack engineering, and customer deployment—with human review, observability, and data controls built into the design.

**From customer problem → system design → implementation → deployment.**

## Engineering depth

| Area | What I work with |
| --- | --- |
| **Agentic AI** | LangChain, custom orchestration, context across channels, and human-in-the-loop workflows |
| **Retrieval & knowledge systems** | Retrieval-augmented generation (RAG), vector search, and source-grounded answers |
| **Document intelligence** | OCR and NLP pipelines for document extraction and validation |
| **AI governance & quality** | PHI/PII redaction, audit trails, LLM evaluation, and observability |
| **Application engineering** | Python, FastAPI, TypeScript, React, Node.js, and PostgreSQL |
| **Cloud & delivery** | AWS, Docker, CI/CD, enterprise integrations, and customer implementation |

## Featured private AI engineering projects

I focus on the engineering behind useful AI: controlled tool execution, permission-aware knowledge access, and reliable business workflows. The repositories below are private; these summaries describe their scope and current stage.

### Helmzon — Backend for AI-assisted clinic workflows

**Go · PostgreSQL · Flutter/Dart · Tool APIs · Transactional outbox**  
**Stage: Backend and application implemented; live voice-provider integration remains pending.**

An operational platform connecting appointment workflows, staff decisions, and the backend tools needed by a voice assistant.

- Implemented call-scoped tool access for clinic context, patient matching, appointment requests, callbacks, and staff handoffs, with clinic boundaries enforced by the backend.
- Kept appointment approval with doctors and sensitive patient access behind identity verification; model-facing tools cannot approve appointments or access finance operations.
- Built durable command dispatch with idempotency and explicit unknown-outcome handling, so interrupted or ambiguous provider actions are reconciled instead of blindly repeated.

**Engineering focus:** Connecting AI tools to real business state while preserving authorization, human decisions, and recoverable failure behavior.

### Northstar Knowledge — Permission-aware enterprise RAG

**Architecture: Python/FastAPI · PostgreSQL/pgvector · React/TypeScript · Hybrid retrieval**  
**Stage: Architecture and evaluation design; implementation planned.**

Designed an enterprise knowledge assistant for account teams to answer customer questions from documents, tickets, and call notes without crossing account or role boundaries.

- Specified server-side authorization before keyword/vector retrieval, reranking, and model context, with access rechecked when citations and source previews are opened.
- Defined answer policies for conflicting evidence, stale information, and the distinction between customer requests, estimates, and approved commitments.
- Designed an evaluation plan using synthetic customer data to assess retrieval quality, citation support, permission revocation, and prompt injection; measured results are not yet available.

**Engineering focus:** Treating access control and evidence quality as core retrieval requirements.

### Aapesey — Local permission controls for AI tools

**Architecture: Go · MCP · Tauri · React/TypeScript · SQLite**  
**Stage: Product specification and technical architecture; implementation planned.**

Designed a local permission checkpoint for supported AI tool connections, starting with a typed filesystem broker and explicitly enrolled project folders.

- Specified deterministic authorization, one-time approvals tied to the exact action, bounded session grants, and explicitly saved permissions.
- Defined process boundaries, typed tool contracts, audit records, and recovery behavior for interrupted operations.
- Documented the protection boundary: controls apply to actions routed through the managed connection; separate terminals and unrelated tools remain outside its scope.

**Engineering focus:** Making agent permissions explicit, reviewable, and bounded before execution.

---

## Selected professional experience

- **Agentic customer journeys at Ushur:** Worked on the Agentic Experience Framework using LangChain and custom orchestration across SMS, email, voice, and web, including human review, sensitive-data redaction, audit trails, and LLM quality monitoring.
- **Document intelligence at Ushur:** Built OCR/NLP workflows for document extraction and validation.
- **Platform engineering at Veltris:** Designed partner integration capabilities and worked on anomaly detection and structured logging.
- **Cloud applications at Wavelabs:** Delivered full-stack applications with AWS messaging integrations, Docker, and CI/CD.
- **Computer vision at ByteForce:** Built applications around PPE detection and supported deployment at GMR Cargo, Hyderabad International Airport.

## Public projects & technical notes

These repositories share project concepts and documentation; their current public contents are described below.

| Repository | Focus | Current public contents |
| --- | --- | --- |
| [Ask-My-Docs](https://github.com/devravisanapala/Ask-My-Docs) | Domain-specific document Q&A with grounded, cited responses | Project brief |
| [LocalMind Automations](https://github.com/devravisanapala/localmind-automations) | Local AI workflows and agentic automation with Ollama | Architecture and automation guide |

## How I approach AI engineering

- Start with the customer workflow and a concrete definition of success.
- Connect models to useful applications, data, and tools.
- Make human review and operational visibility part of the system.
- Evaluate quality alongside latency, cost, and reliability.
- Stay involved through integration and deployment.

[Connect on LinkedIn](https://www.linkedin.com/in/sanapalaravi/)
