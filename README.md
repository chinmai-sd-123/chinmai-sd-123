<div align="center">

# Chinmai S D

**AI engineer who builds the systems behind AI.**

I work on reliability, evaluation, and observability for production AI, and on the backend
infrastructure that makes those systems hold up.

[Portfolio](https://www.chinmai-sd.me/) &nbsp;·&nbsp;
[LinkedIn](https://linkedin.com/in/chinmai-sd) &nbsp;·&nbsp;
[Email](mailto:chinmaisdinesh@gmail.com)

</div>

---

### What I'm focused on

Most "AI works" demos fall apart in production. I spend my time on the unglamorous parts that
decide whether they actually hold: knowing *why* an answer was wrong, catching failures before
users do, keeping cost and latency honest, and making the data pipeline underneath trustworthy.

B.E. Information Science at DSCE Bengaluru (CGPA 8.82, 2027). Published at IEEE ICTBIG 2025.

---

### Selected work

**[TraceroAI](https://traceroai.tech) — reliability infrastructure for production AI**
A RAG evaluation and observability platform: a Python SDK on PyPI feeds a FastAPI backend and a
Next.js dashboard. Instead of flagging a generic "hallucination," it tells you *which* stage
failed: retrieval, context, or generation. The evaluation engine runs in two tiers, fast
embedding relevance scoring inline and LLM-as-Judge groundedness checks asynchronously, with a
LangGraph agent that proposes fixes.
`Python SDK` · `FastAPI` · `LangGraph` · `Redis` · `Next.js`

**[LogScope](https://github.com/chinmai-sd-123/LogScope) — log intelligence and incident triage**
A terminal tool that tails logs live, groups thousands of near-identical lines into a handful of
patterns with the Drain algorithm, flags error spikes with plain statistics, and searches history
over SQLite FTS5. Includes a distributed mode where agents ship logs to a central server with
at-least-once delivery and idempotent writes, so nothing is lost and nothing is double-counted.
Single asyncio event loop with backpressure throughout. 100+ tests.
`Python` · `asyncio` · `SQLite/FTS5` · `custom TCP protocol`

**[SignalStack](https://github.com/chinmai-sd-123/SIgnal_Stack) — grounded candidate evaluation**
Evaluates engineers against real evidence pulled from their GitHub and coding profiles, then
validates each generated assessment against the retrieved code so the output stays grounded.
Batched, outcome-level evaluation cut LLM call volume by roughly 5x and token cost by about 60%.
`FastAPI` · `PostgreSQL` · `Redis` · `OpenAI`

**[Astronaut Health Monitoring](https://github.com/chinmai-sd-123/astronaut_space_health) — real-time ML, IEEE published**
A streaming inference pipeline classifying physiological risk under a 50 ms latency target.
XGBoost over 49K records with 68 engineered features, plus Isolation Forest and Prophet for
anomaly detection and forecasting. 93.1% accuracy.
Published at IEEE ICTBIG 2025 · [DOI](https://doi.org/10.1109/ICTIBG68706.2025.11323855)
`FastAPI` · `XGBoost` · `Isolation Forest` · `Prophet`

<details>
<summary>Other work</summary>

<br/>

- **[EvidenceGPT](https://github.com/chinmai-sd-123/EvidenceGPT)** — verifiable research assistant with an evidence graph and human oversight.
- **[Structured Data Extractor API](https://github.com/chinmai-sd-123/Structured_Data_Extractor_API)** — production-oriented backend that extracts structured company data with validated outputs.
- **[RAG Playground](https://github.com/chinmai-sd-123/rag_playground)** — a from-scratch RAG sandbox with LangChain and Chroma.

</details>

---

### Tools I reach for

**AI / ML**&nbsp; Python · PyTorch · scikit-learn · XGBoost · Hugging Face Transformers
**LLM systems**&nbsp; RAG · LangGraph · LangChain · LLM-as-Judge · structured outputs · OpenAI / Gemini APIs
**Backend**&nbsp; FastAPI · REST · Redis · PostgreSQL · background workers · Docker · CI/CD
**Observability**&nbsp; Prometheus · token / cost / latency tracking · vector search
