AI infrastructure engineer. Building production multi-agent systems on LangGraph, Gemini, and Redis — multi-tenant, multi-role, multi-timezone.

---

## What I'm working on

- **Multi-agent AI platform** — role-based CrewAI agents (Founder / Manager / Specialist) with long-term memory (Mem0 + Qdrant), Gemini context caching, and timezone-aware task scheduling. Runs in production across multiple organizations.
- **Gemini context caching at scale** — pre-baking tools + system instructions into `CachedContent` per role per scenario, achieving a 75% token cost reduction on cached prompts across all agent turns.
- **LangGraph checkpoint management** — custom interrupt-safe pruning strategy (`keep_last=N`) to prevent tool re-execution in multi-tool interrupt chains on `AsyncRedisSaver`.

---

## Open source contributions

| PR | Repo | What |
|---|---|---|
| [#1619](https://github.com/langchain-ai/langchain-google/pull/1619) | `langchain-ai/langchain-google` | Strip `tools`/`tool_config`/`system_instruction` from request when `cached_content` is set — production-tested fix for Gemini context caching with tool-calling agents |
| [#159](https://github.com/redis-developer/langgraph-redis/issues/159) | `redis-developer/langgraph-redis` | Implementing `aprune()` / `prune()` with `keep_last=N` strategy for interrupt-safe checkpoint pruning in `AsyncRedisSaver` |

---

## Stack

**Core:** Python · FastAPI · LangGraph · CrewAI · LangChain  
**AI:** Gemini (context caching) · OpenAI (Whisper, TTS) · Mem0 · Qdrant  
**Infra:** PostgreSQL · MongoDB · Redis · Celery · Docker · SQLAlchemy (async)  
**Tooling:** uv · Alembic · Ruff · mypy · pytest

---

## Reach me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mukhsin-mukhtorov-58b26221b/)
[![X](https://img.shields.io/badge/X-000000?style=flat&logo=x&logoColor=white)](https://x.com/MukhsinMM7)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:muxsinmuxtorov01@gmail.com)
[![Wakatime](https://wakatime.com/badge/user/60731bfe-5801-4003-b6ab-b7db12ed73d0.svg)](https://wakatime.com/@60731bfe-5801-4003-b6ab-b7db12ed73d0)
