# Hi, I'm Nithish Yenaganti

I build backend systems and developer tools at a small AI consulting startup, mostly in **Python, TypeScript, Go and SQL**. I'm looking for **backend engineering and AI infrastructure** roles.

## What I've been building

**It started with a messy problem:** every app wanted its own AI provider keys and its own API format. So I built **[ProxyLLM](https://github.com/Nithish-Yenaganti/proxyllm)** (Python / FastAPI), one OpenAI-compatible gateway for Anthropic and Fireworks. Apps get virtual keys, the real keys stay on the server, and you can preview a translated request before it's sent.
[Run locally](https://github.com/Nithish-Yenaganti/proxyllm#run-locally) · [Architecture](https://github.com/Nithish-Yenaganti/proxyllm/blob/main/ARCHITECTURE.md)

**Then I got tired of leaving the terminal to read docs,** so I built **[Shine](https://github.com/Nithish-Yenaganti/shine)** (Go). It previews Markdown in the shell and checks broken links, missing alt text and heading structure.
[Watch the demo](https://youtu.be/0RvUFqgH8io) · [Install v0.1.2](https://github.com/Nithish-Yenaganti/shine/releases/tag/v0.1.2)

**Along the way I found a bug in LiteLLM.** Passing an existing file to RAG ingestion reported success but never attached the file. I fixed it, added tests, and [the PR was merged](https://github.com/BerriAI/litellm/pull/30628) on June 18, 2026.
[Read the case study](https://github.com/Nithish-Yenaganti/Nithish-Yenaganti/blob/main/case-studies/litellm-rag-ingestion.md) · [All my public PRs](https://github.com/search?q=author%3ANithish-Yenaganti+is%3Apr+is%3Apublic&type=pullrequests)

## With teams

- **TimesOfSF:** backend features for scheduling, subscriptions, health checks and article APIs (private repo).
- **Nirnaya** *(in progress, private):* a multi-agent research app where specialist agents and a critic write reports that show their sources and gaps.

Found a bug in one of my projects? Open an issue in that repo with the version and a small example.
