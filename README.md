# Hi, I'm Nithish

Software engineer shipping production AI systems
for clients across industries. I build across the full stack — from distributed
agentic pipelines and RAG systems on GCP to MCP servers and fine-tuned LLMs —
with a focus on reliability, scalability, and real-world impact.

---
 
## Currently Working On

- Making improvements to **Nirnaya**, my AI research app for companies and open-source projects.
- Stress testing **ProxyLLM**, my Python gateway for Fireworks and Anthropic models.

## Projects

### Nirnaya

An AI research app that turns a company or open-source project's name or website into a source-backed report. Four workers research its team, funding, technology, and competitors in parallel, then combine their findings with source links, supporting quotes, and clear notes about missing information.

Includes a web interface, saved results, and spending controls. I'm currently making improvements; real-world research testing and cloud deployment are still pending.

### ProxyLLM

A Python project that gives applications one shared API for Fireworks and Anthropic models. Each application gets its own virtual key, while the real provider keys stay on the server.

Built with FastAPI and SQLite, it includes access controls, request limits, streaming responses, reusable response caching, and usage and estimated cost tracking. A local dashboard and automated tests support the project as a learning and portfolio effort. I'm currently stress testing it.

---

## Open Source
 
**[litellm](https://github.com/BerriAI/litellm)** — Python SDK and AI Gateway to call 100+ LLMs · ⭐ 50k+
 
[**fix(rag): attach existing OpenAI file ids**](https://github.com/BerriAI/litellm/pull/30628) — Tracked down a silent data loss bug in the RAG ingestion pipeline: passing an existing `file_id` to the OpenAI path returned a success response without actually attaching the file to the vector store. Fixed the attach logic, added a provider contract so unsupported backends fail clearly instead of silently, and wrote tests covering all three code paths.
 
---


[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)](https://langchain.com/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![GCP](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=for-the-badge&logo=pinecone&logoColor=white)](https://www.pinecone.io/)
[![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/)

