# Hi, I'm Nithish

I build AI infrastructure and developer tools: LLM gateways, retrieval workflows, and MCP tools that help coding agents work with repository context. My public work spans Python, TypeScript, and Go.

## Selected public projects

### [Shine](https://github.com/Nithish-Yenaganti/shine)

A terminal Markdown previewer and docs checker. Preview a README, navigate its outline, and check local links, image alt text, and heading structure without leaving the shell.

[Watch the demo](https://youtu.be/0RvUFqgH8io) · [Install v0.1.2](https://github.com/Nithish-Yenaganti/shine/releases/tag/v0.1.2) · [Quick start](https://github.com/Nithish-Yenaganti/shine#install)

### [PromptIT](https://github.com/Nithish-Yenaganti/PromtIT)

A local MCP preflight tool that checks a coding request against Git state and returns a structured risk decision. Policies cover migrations, authentication, deployment, dependencies, and secret-looking changes. Enforcement depends on the host calling the tool and honoring its decision.

[Setup and examples](https://github.com/Nithish-Yenaganti/PromtIT#quick-start)

### [Aksi](https://github.com/Nithish-Yenaganti/Aksi)

A local MCP context tool that maps repository structure, tracks stale summaries, and gives coding agents specific context to refresh. A static viewer brings together structure, architecture, and runtime-flow models; the host supplies grounded summaries.

[Install from source](https://github.com/Nithish-Yenaganti/Aksi#install-for-mcp)

## Open-source contribution

**[LiteLLM: fix existing-file RAG ingestion](https://github.com/BerriAI/litellm/pull/30628)** — merged June 18, 2026.

Passing an existing OpenAI `file_id` could report successful ingestion without attaching the file to its vector store. I implemented the attachment path, made unsupported provider behavior explicit, and added regression tests for the success and failure cases. The PR received maintainer approval and passed all 73 checks before merging.

[Read the debugging case study](case-studies/litellm-rag-ingestion.md) · [Browse my public pull requests](https://github.com/search?q=author%3ANithish-Yenaganti+is%3Apr+is%3Apublic&type=pullrequests)

## Current private projects

These repositories are private; the descriptions below explain the work, but are not public demos or benchmark results.

- **Nirnaya:** an AI due-diligence app with four parallel research workers covering a project's team, funding, technology, and competitors. Reports include sources, supporting quotes, and evidence gaps, with persistent results and spending controls.
- **ProxyLLM:** a Python gateway built with FastAPI and SQLite for Fireworks and Anthropic, with per-app virtual keys, streaming, rate limiting, caching, and usage and estimated-cost tracking.

## Working with my projects

For reproducible bugs or feature requests, use the issue tracker linked from each public repository. Include your version, a minimal example, expected behavior, and actual output, with credentials and private data removed.
