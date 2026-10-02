# Hi, I'm Nithish Yenaganti

I work at a small AI consulting startup and build backend systems and developer tools. My work spans AI gateways and terminal tools, using **Python, TypeScript, Go, and SQL**.

I'm interested in **backend engineering and AI infrastructure opportunities**. Below are projects you can run, a merged open-source contribution, and a little about my collaborative work.

## Featured projects

### [ProxyLLM](https://github.com/Nithish-Yenaganti/proxyllm) · Python / FastAPI / SQLite

A gateway that lets applications call Anthropic and Fireworks through one OpenAI-compatible API. Each application uses a virtual key while provider credentials stay on the server. It handles provider permissions, request translation, streaming, per-key caching, and usage tracking.

**A feature to try:** inspect the translated request before sending it, using the same preparation code as execution and without calling a provider.

Designed for a single host, with mock and real-provider testing. The management dashboard stays local; public deployment and high availability are outside the current version.

[Run locally](https://github.com/Nithish-Yenaganti/proxyllm#run-locally) · [Architecture](https://github.com/Nithish-Yenaganti/proxyllm/blob/main/ARCHITECTURE.md) · [Request inspection](https://github.com/Nithish-Yenaganti/proxyllm/blob/main/docs/inspection.md)

### [Shine](https://github.com/Nithish-Yenaganti/shine) · Go

A terminal Markdown previewer and docs checker. Preview a README, navigate its outline, and check local links, image alt text, and heading structure without leaving the shell.

[Watch the demo](https://youtu.be/0RvUFqgH8io) · [Install v0.1.2](https://github.com/Nithish-Yenaganti/shine/releases/tag/v0.1.2) · [Quick start](https://github.com/Nithish-Yenaganti/shine#install)

## Open-source contribution

**[LiteLLM: fix existing-file RAG ingestion](https://github.com/BerriAI/litellm/pull/30628)** — merged June 18, 2026.

Passing an existing OpenAI `file_id` could report successful ingestion without attaching the file to its vector store. I implemented the attachment path, made unsupported provider behavior explicit, and added regression tests for the success and failure cases. The change was reviewed and merged by the maintainers.

[Read the debugging case study](https://github.com/Nithish-Yenaganti/Nithish-Yenaganti/blob/main/case-studies/litellm-rag-ingestion.md) · [Browse my public pull requests](https://github.com/search?q=author%3ANithish-Yenaganti+is%3Apr+is%3Apublic&type=pullrequests)

## Collaborative work and ongoing research

- **TimesOfSF:** contributed backend features covering scheduling, subscriptions, health checks, and article APIs through reviewed pull requests in a private team repository.
- **Nirnaya — private, in progress:** a multi-agent company research app using LangGraph, FastAPI, Redis, and Next.js. A supervisor coordinates four specialists and a critic; reports expose sources, supporting passages, and evidence gaps. Live evaluation and deployment are not presented as completed results.

For project questions or reproducible bugs, use the relevant repository's issue tracker. Include the version, expected behavior, and a minimal example with credentials and private data removed.
