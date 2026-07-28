### Hi, I'm Shree 👋

AI/ML Engineer focused on Generative AI, multi-agent systems, and RAG architectures — I like building things that go beyond a notebook and actually run as a service.

🔭 Currently building agentic workflows with LangGraph and fine-tuning open-source LLMs for domain-specific tasks
🧠 Interested in: multi-agent orchestration, hybrid retrieval, efficient fine-tuning (QLoRA/PEFT)
📫 Reach me: shreelondhe2004@gmail.com | [LinkedIn](https://linkedin.com/in/shree-londhe-b082b2245)

## 🚀 Featured Projects

### 🤖 [Multi-Agent Research Assistant](https://github.com/Shree-2004/Multi-Agent-Research-Assistant)
A production-style multi-agent system built on LangGraph StateGraph — 4 specialized agents (Researcher, Analyst, Writer, Critic) coordinating through shared state.

- Reflection loop: Critic runs a 5-point verification checklist, routing back to the Analyst for up to 2 self-correction cycles
- Custom latency/quality benchmark suite tracking citation frequency and performance drift over time
- Stack: LangGraph, Gemini 2.0, Tavily, ArXiv API

### 📊 [SEBI/BSE Financial Filing RAG Analyzer](https://github.com/Shree-2004/SEBI-BSE-Financial-Filing-RAG)
A hybrid-retrieval RAG system built for dense financial documents — tables, filings, and mixed layouts.

- Combines dense vector search (BAAI/bge-base-en-v1.5) with sparse BM25 for precision on both semantic queries and exact figures
- Structure-aware ingestion using pdfplumber + Tesseract OCR to preserve table integrity through chunking
- CrossEncoder re-ranking + citation verification layer to keep generation grounded in source text
- Stack: Qdrant, FastAPI, BM25, PyTorch

### 💰 [Domain Fine-Tuned Finance LLM](https://github.com/Shree-2004/Finance-llm)
Fine-tuned Mistral-7B-Instruct on localized Indian personal finance data.

- QLoRA (4-bit NormalFloat) fine-tuning — 4× memory footprint reduction
- Ran a systematic LoRA rank ablation (r=8/16/32) tracked in MLflow
- +88.6% improvement in target keyword coverage after tuning
- Merged adapters back into 16-bit weights, pushed to HuggingFace Hub, deployed via Gradio
- Stack: Mistral-7B, QLoRA, MLflow, HuggingFace

## 🛠️ Tech Stack

**Languages & Core:** Python · C++ · SQL · Git
**ML/DL:** PyTorch · TensorFlow · Scikit-learn · HF Transformers · PEFT/LoRA
**GenAI:** LangGraph · LangChain · LlamaIndex · CrewAI · OpenAI API · Gemini 2.0
**Retrieval/Storage:** Qdrant · FAISS · ChromaDB · Pinecone · PostgreSQL · BM25
**MLOps:** FastAPI · Docker · MLflow · Weights & Biases · Streamlit · Gradio

⭐ Open to AI/ML Engineer and Applied ML roles — feel free to reach out!
