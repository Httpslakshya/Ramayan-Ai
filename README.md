# 🕉️ Ramayan AI

Ramayan AI is an AI-powered RAG (Retrieval-Augmented Generation) chatbot that allows users to interact with the Ramayan using natural language.

Built using LangChain, Qdrant, HuggingFace embeddings, and Groq LLMs, the system semantically retrieves relevant passages from the Ramayan and generates contextual responses grounded in the source material.

Instead of sending the entire PDF to the AI model every time, Ramayan AI performs semantic similarity search on vector embeddings to fetch only the most relevant context before generating an answer.

---

## ✨ Features

- 📖 Chat with the Ramayan conversationally
- 🔍 Semantic search using vector embeddings
- 🧠 RAG (Retrieval-Augmented Generation) architecture
- ⚡ Fast AI responses using Groq Llama models
- 🆓 Free local embeddings using Sentence Transformers
- 🗂️ Qdrant vector database integration
- 📄 Multi-PDF support
- 🎯 Context-aware answers with source references
- 📚 Handles large PDFs efficiently

---

# 🏗️ Architecture

```text
User Query
    ↓
Semantic Similarity Search
    ↓
Relevant Ramayan Chunks
    ↓
Context Injection
    ↓
Groq LLM
    ↓
Final AI Response
```

# 🧠 RAG Pipeline

Ramayan PDF
```text      ↓
Text Chunking
      ↓
MiniLM Embeddings
      ↓
Qdrant Vector Database
      ↓
Semantic Retrieval
      ↓
Relevant Context
      ↓
LLM Response Generation
```

# 🛠️ Tech Stack

Python
LangChain
Qdrant
HuggingFace Sentence Transformers
Groq API
PyPDFLoader

# 💬 Example Queries
```text
Who is Hanuman?
Describe Lord Rama's appearance
What happened during Sita Haran?
Tell me about Lakshman's loyalty
```

# 🚀 Future Improvements

Conversational memory
Voice interaction
Character-specific search
Hindi/Sanskrit support
Web interface
Citation highlighting
Hybrid search

# 🧠 What is RAG?

RAG (Retrieval-Augmented Generation) retrieves relevant information from documents before sending context to the AI model.

This makes responses:

more accurate
context-aware
scalable
efficient for large documents

# 🙌 Credits
Valmiki Ramayan
Project Gutenberg edition
LangChain
Qdrant
HuggingFace
Groq
