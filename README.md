## Hi, I'm Shree 👋

I'm an AI/ML engineer who builds LLM systems and then checks whether they actually work. Most of my projects come with a benchmark. Most of my best results came from finding a number that was wrong and fixing it: a lenient eval metric, a judge scoring runs that never happened, a "falsified" claim the data couldn't support.

I work on **RAG over messy real-world documents**, **multi-agent pipelines**, and **evaluation harnesses for LLM agents**. I graduated in 2026 with a B.Tech in IT.

[Portfolio](https://portfolio-bice-nine-ekrh7ppg1i.vercel.app) · [LinkedIn](https://linkedin.com/in/shree-londhe-b082b2245) · shreelondhe2004@gmail.com

---

### Featured work

**[FinFiling RAG](https://github.com/Shree-2004/SEBI-BSE-Financial-Filing-RAG-Analyzer)**: question answering over Indian SEBI/BSE financial filings · [live demo](https://sebi-bse-financial-filing-rag-analy.vercel.app)
- **93.5% strict accuracy** (116/124) across 13 companies. It says so instead of inventing a number on 6/6 unanswerable questions.
- I found the old 95.6% score came from a lenient metric (the real figure was 29%). Rebuilding the parsing with Docling brought it to 87% on the same questions.
- A tool-using agent handles comparisons and growth questions (13/13 vs 5/13 for plain RAG). A cell-level verifier catches 85% of wrong figures.
- Runs in a 512 MB free tier thanks to ONNX int8 · Qdrant + BM25 hybrid search · FastAPI · Groq

**[stock-judgment-bench](https://github.com/Shree-2004/stock-judgment-bench)**: does an LLM's stock judgement hold up once lookahead leakage is removed?
- 3,690 point-in-time briefs on 41 NSE stocks across 90 windows (2019–2026). **No detectable edge** (rank corr −0.015, 95% CI −0.061 to +0.031).
- Cited figures are 99.98% correct, with 0 fabricated filing citations in 8,804 claims. The model gets the facts right and still can't predict returns.
- Now running as a live, hash-chained prediction ledger, so every call is made after the model's training cutoff.

**[AgentLens](https://github.com/Shree-2004/agentlens)**: a trace debugger that finds the step where a multi-step agent run went wrong
- An LLM judge, scored against hand-labelled traces: **28/30 on the labelled step, 0 false positives**.
- Prompt-injection hardening: a false accusation planted in tool output dropped from 3/3 to 0/3. Code checks every quote the judge cites (89/91 found).

**[Multi-Agent Research Assistant](https://github.com/Shree-2004/Multi-Agent-Research-Assistant)**: a 5-agent LangGraph pipeline (Researcher → Analyst → Writer → Verifier → Critic)
- A Citation Verifier checks each cited claim against its source. This revealed that a revision can make citations *worse*, so a guard ships the best draft, not the last one.
- Retries and graceful degradation · CI-tested · Gemini, Tavily, ArXiv

<sub>Also: [AgentSentinel](https://github.com/Shree-2004/Agentsentinel) (agent red-teaming harness) · [finance-agent](https://github.com/Shree-2004/finance-agent) (Google ADK + MCP) · [Self-Healing RAG](https://github.com/Shree-2004/Self-Healing-RAG) · [Finance-llm](https://github.com/Shree-2004/Finance-llm) (QLoRA on Mistral-7B)</sub>

---

### Tools I use

**LLM & agents:** LangGraph · LangChain · LlamaIndex · CrewAI · OpenAI / Gemini / Groq APIs
**Retrieval:** Qdrant · FAISS · BM25 · cross-encoder reranking · Docling
**ML:** Python · PyTorch · TensorFlow · Hugging Face Transformers · PEFT/QLoRA · scikit-learn
**Shipping:** FastAPI · Docker · ONNX Runtime · GitHub Actions · MLflow · W&B · Streamlit · SQL

Open to AI/ML Engineer and Applied ML roles.
