
# 💡 What is RAGnosis?

**RAGnosis** is an intelligent open-source teaching agent that combines Retrieval-Augmented Generation (RAG) with agentic reasoning. Designed to act as a **personal tutor, course assistant, and academic researcher**, RAGnosis enables:

- Grounded responses backed by your own documents and open academic datasets.
- Memory-augmented multi-turn reasoning and concept tracking.
- Step-by-step explanations, citations, and dynamic question chaining.

It works great in educational settings, research labs, and AI-enhanced LMS tools.

Visit the live demo: [https://shikshaai.site](https://shikshaai.site)

---

## 🔧 Key Features

- ✏️ **Document-Aware Tutor**: Upload textbooks, PDFs, or scraped course content for adaptive questioning.
- ⚙️ **Multi-Agent Teaching**: Use curriculum-planning agents, question generators, and explainer agents collaboratively.
- 📈 **Citation-Based RAG**: Answers include accurate citations from your knowledge base.
- 👤 **User Profiles & Tracing**: Retain student context, progress, and misunderstood concepts.
- 🖊️ **Custom Personas**: Let the AI emulate different educator styles (e.g. Socratic, Khan Academy, IIT Coach).

---

## ⚖️ Architecture Overview

> "Teaching is the art of assisting discovery."

RAGnosis uses the following pipeline to simulate educational reasoning:

```
Student Query ➞ Query Rewriting Agent ➞ Retriever (Semantic + Keyword)
         ➞ Chunk Scoring ➞ Compression Agent ➞ Context-Rich Prompt
         ➞ Reasoning Agent (LLM) ➞ Answer + Citations + Suggested Next Questions
```

### Components

- **Vector Store**: Weaviate, Qdrant, or FAISS
- **Chunkers**: Custom academic chunkers (heading-aware, textbook-optimized)
- **Reasoning Agent**: GPT-4, Claude, or open-weight LLMs (Mixtral, Yi, Zephyr)
- **Persona & Tone Engine**: Adjustable per session or student profile
- **Citation Handler**: Inline citation via Markdown or rich card format

---

## 🚀 Deployment Options

### 1. Quick Start (Docker)

```bash
git clone https://github.com/arrnaya/RAGnosis.git
cd ragflow
docker-compose up --build
```

Then visit: `http://localhost:7860`

### 2. Lightweight Deployment (for schools or Raspberry Pi)

- Use Ollama + Mixtral
- Swap embedding model to `bge-small-en` or `e5-base`
- Run frontend with `yarn dev` or Vite
- Serve over LAN or internal network

### 3. Cloud Deploy (Educational SaaS)

- Use S3 / GCS for file upload
- Supabase or Firebase for auth & tracking
- Optional: Integrate with Moodle, Canvas via LTI or API

---

## 🌐 Website & Docs

- Homepage: [https://shikshaai.site](https://shikshaai.site)
- Documentation: [https://shikshaai.site/docs](https://shikshaai.site/docs)
- Demo Playground: [https://shikshaai.site/play](https://play.shikshaai.site)

---

## 🤝 Join the Community

- Discord: [#](#)
- Twitter/X: [@shikshaai](https://twitter.com/shikshaai)
- Email: [hello@shikshaai.site](mailto\:hello@shikshaai.site)

---

## 🌟 License

Apache 2.0 with educational clause: you can use, modify, and redistribute RAGnosis as long as it is not used for surveillance, behavioral scoring, or exploitative advertising in educational settings.

---

## 💪 Contributing

We welcome contributors in:

- Educational AI agents
- NLP and chunking improvements
- Frontend UX for students/teachers
- Dataset preparation (open curriculum, lecture PDFs)

Open issues or join the discussion on [GitHub](https://github.com/arrnaya/RAGnosis/issues)

---

Made with ❤️ by [ShikshaAI](https://shikshaai.site)
