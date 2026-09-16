# Hi, I'm Nithish

I'm a software engineer building production AI systems for clients across industries. I work across the full stack, including distributed agent pipelines, RAG systems on GCP, MCP servers, and fine-tuned LLMs. I care about making these systems reliable, able to scale, and useful in practice.

## What I'm working on

I'm making improvements to **Nirnaya** and testing benchmarks for **ProxyLLM**.

## Projects

### Nirnaya

Nirnaya is an AI due diligence app with four parallel research workers that analyze a company or open-source project's team, funding, technology, and competitors to produce reports with source links, supporting quotes, and evidence gaps. It includes a web interface, persistent results, and spending controls; real-world research validation and cloud deployment are pending.

### ProxyLLM

ProxyLLM is a Python LLM gateway built with FastAPI and SQLite that provides a unified API for Fireworks and Anthropic, with per-app virtual keys and server-side provider credentials. It supports access control, rate limiting, streaming, response caching, usage and estimated cost tracking, plus a local dashboard and automated tests.

## Open Source

**[litellm](https://github.com/BerriAI/litellm)** — Python SDK and AI Gateway to call 100+ LLMs · ⭐ 50k+

[**fix(rag): attach existing OpenAI file ids**](https://github.com/BerriAI/litellm/pull/30628)

I tracked down a silent data loss bug in the RAG ingestion pipeline: passing an existing `file_id` to the OpenAI path returned a success response without attaching the file to the vector store. I fixed the attach logic, added a provider contract so unsupported backends fail clearly, and wrote tests for all three code paths.

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
