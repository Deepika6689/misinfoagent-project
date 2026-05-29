# 🛡️ Misinformation Audit Agent
##.

### LangGraph + RAG + NLP + Fact Verification System

An AI-powered misinformation detection and fact-checking system that analyzes articles claim-by-claim, retrieves supporting evidence from trusted sources, and generates a structured credibility audit report automatically.

The project combines **LangGraph workflows**, **Retrieval-Augmented Generation (RAG)**, **Natural Language Inference (NLI)**, and **real-time web search** to identify misinformation efficiently.

---

# 🌟 Features

- ✅ Automated claim extraction from articles
- ✅ Claim-by-claim fact verification
- ✅ Contradiction detection within articles
- ✅ Evidence retrieval using ChromaDB RAG
- ✅ Real-time web search using Serper API
- ✅ DeBERTa-v3 NLI classification
- ✅ Structured credibility audit reports
- ✅ Local LLM support using Ollama
- ✅ Interactive animated frontend using GSAP + FastAPI

---

# 🧠 Architecture

```text
Article Text
     │
     ▼
┌─────────────────┐
│ Claim Extractor │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ RAG Retriever   │
│ (ChromaDB)      │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Web Search      │
│ (Serper API)    │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ NLI Verifier    │
│ DeBERTa-v3      │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Report Generator│
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Contradiction   │
│ Detection       │
└─────────────────┘
```

---

# 🧩 Tech Stack

## Backend
- Python
- FastAPI
- LangGraph
- LangChain

## AI / NLP
- DeBERTa-v3 NLI
- Retrieval-Augmented Generation (RAG)
- Ollama Local LLMs

## Database & Retrieval
- ChromaDB

## Frontend
- HTML
- CSS
- JavaScript
- GSAP Animations

## APIs & Tools
- Serper API
- Wikipedia Tool

---

# 📁 Project Structure

```bash
root/
│── frontend/                 # Frontend application
│── static/                   # Static assets
│── chroma_db/                # ChromaDB vector database
│── custom_docs/              # Custom documents for RAG
│── app.py                    # Main app
│── server.py                 # FastAPI server
│── graph.py                  # LangGraph workflow
│── ingest.py                 # RAG ingestion pipeline
│── finetune.py               # NLI model fine-tuning
│── run_trace.py              # Workflow tracing
│── requirements.txt          # Dependencies
│── Dockerfile                # Docker setup
└── README.md
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/Deepika6689/misinfoagent-project.git
cd misinfoagent-project
```

---

## 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

---

## 3️⃣ Activate Environment

### Windows

```bash
venv\Scripts\activate
```

### macOS/Linux

```bash
source venv/bin/activate
```

---

## 4️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 5️⃣ Configure Environment Variables

Create a `.env` file:

```env
SERPER_API_KEY=your_api_key
OPENAI_API_KEY=your_api_key
```

---

## 6️⃣ Build the RAG Database

```bash
python ingest.py
```

---

## 7️⃣ Run the Application

```bash
uvicorn server:app --reload
```

Open:

```bash
http://localhost:8000
```

---

# 🚀 How It Works

1. User submits an article
2. Claims are extracted automatically
3. Relevant evidence is retrieved using:
   - ChromaDB RAG
   - Serper web search
4. DeBERTa-v3 verifies each claim
5. Claims are classified as:
   - Supported
   - Refuted
   - Not Enough Information
6. A structured misinformation audit report is generated

---

# 🔬 AI Concepts Used

- LangGraph Workflow Automation
- Retrieval-Augmented Generation (RAG)
- Natural Language Processing (NLP)
- Natural Language Inference (NLI)
- AI Agent Systems
- Vector Databases
- Local LLM Deployment

---

# 🔮 Future Enhancements

- 🌐 Multi-language support
- 📄 PDF upload support
- 📊 Analytics dashboard
- ☁️ Cloud deployment
- 🔐 User authentication
- 📱 Mobile responsiveness

---

# 👩‍💻 Author

## Deepika
AIML Engineering Student  
Passionate about AI, NLP, LLMs, and Full Stack Development

---

# ⭐ Support

If you like this project, give it a ⭐ on GitHub.

---

# 🤝 Contributor

- **@sourabhsp23** – Support and contributions to the project

---
