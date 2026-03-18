# 🧠 AI Document Intelligence System

> An intelligent platform to upload, summarize, and chat with your documents and videos — powered by RAG, LLMs, and multilingual TTS.

---

## ✨ Features

- 📄 **Document Summarization** — Upload PDFs, DOCX, PPTX, XLS, CSV and get instant AI-generated summaries
- 🎥 **Video Summarization** — Extract key insights from video content automatically
- 💬 **AI Chat (RAG)** — Ask questions about your uploaded content using Retrieval-Augmented Generation
- 🔊 **Text-to-Speech** — Listen to summaries in English, Hindi, and Kannada
- 🌐 **Translation Support** — Multilingual output for broader accessibility
- 📜 **History Tracking** — Revisit all past uploads, chats, and summaries
- ⚡ **Fast & Accurate** — Adaptive processing strategies based on content complexity

---

## 🛠 Tech Stack

**Frontend**
- React + TypeScript
- Framer Motion
- Tailwind CSS + shadcn/ui

**Backend**
- Python (FastAPI)
- LangChain + OpenAI GPT
- ChromaDB (Vector Store)
- Sentence Transformers (`all-MiniLM-L6-v2`)
- gTTS (Multilingual Text-to-Speech)
- NVIDIA Audio2Face

---

## 📁 Project Structure

```
├── frontend/
│   ├── Home.tsx          # Landing page
│   ├── Upload.tsx        # File upload interface
│   ├── Chat.tsx          # RAG chat interface
│   ├── Summary.tsx       # Summary viewer
│   └── History.tsx       # Past sessions
│
├── backend/
│   ├── rag_engine.py         # Hybrid RAG with query expansion
│   ├── summarizer.py         # Adaptive text summarization
│   ├── document_processor.py # Multi-format file parsing
│   ├── video_integration.py  # Video processing pipeline
│   ├── tts_engine.py         # Multilingual TTS
│   ├── translator.py         # Language translation
│   ├── animation_engine.py   # Character animation (Audio2Face)
│   ├── database_manager.py   # Storage & history
│   └── config.py             # App configuration
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js ≥ 18
- Python ≥ 3.10
- OpenAI API Key
- (Optional) NVIDIA Audio2Face for animated summaries

### 1. Clone the repo

```bash
git clone https://github.com/your-username/ai-summarization-system.git
cd ai-summarization-system
```

### 2. Backend setup

```bash
cd backend
pip install -r requirements.txt
cp .env.example .env   # Add your API keys
python main.py
```

### 3. Frontend setup

```bash
cd frontend
npm install
npm run dev
```

---

## 🔑 Environment Variables

```env
OLLAMA_MODEL=llama3.2
OLLAMA_BASE_URL=http://localhost:11434
NVIDIA_API_KEY=your_nvidia_key
AUDIO2FACE_URL=http://localhost:8011
```

---

## 📦 Supported File Types

| Type | Formats |
|------|---------|
| Documents | `.pdf`, `.docx`, `.pptx`, `.xls`, `.xlsx`, `.csv` |
| Images | `.png`, `.jpg`, `.jpeg` |
| Audio | `.mp3`, `.wav`, `.ogg` |
| Video | `.mp4` and more |

---

## 🌍 Supported Languages

- 🇬🇧 English
- 🇮🇳 Hindi (हिंदी)
- 🇮🇳 Kannada (ಕನ್ನಡ)

---



<p align="center">Built with ❤️ using React, Python, LangChain & OpenAI</p>
