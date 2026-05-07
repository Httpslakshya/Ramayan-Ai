Ramayan AI 🕉️🤖
An AI-powered RAG (Retrieval-Augmented Generation) chatbot built using LangChain, Qdrant, HuggingFace embeddings, and Groq LLMs that allows users to chat with the Ramayan PDF semantically.
The project retrieves relevant passages from the Ramayan and generates grounded responses using AI instead of sending the entire PDF to the model every time.

✨ Features


📖 Chat with the Ramayan PDF


🔍 Semantic search using vector embeddings


🧠 RAG architecture (Retrieval-Augmented Generation)


⚡ Fast inference using Groq Llama models


🆓 Free local embeddings using Sentence Transformers


🗂️ Qdrant Vector Database integration


📄 Multi-PDF support


🎯 Context-aware answers with page references



🏗️ Architecture
PDF ↓Text Chunking ↓Embeddings (MiniLM) ↓Qdrant Vector Database ↓Similarity Search ↓Relevant Context Retrieval ↓Groq LLM ↓Final AI Answer

🛠️ Tech Stack


Python


LangChain


Qdrant


HuggingFace Sentence Transformers


Groq API


PyPDFLoader



📦 Installation
1. Clone Repository
git clone https://github.com/yourusername/ramayan-ai.gitcd ramayan-ai

2. Create Virtual Environment
python -m venv .venv
Activate:
Windows
.venv\Scripts\activate
Linux / Mac
source .venv/bin/activate

3. Install Dependencies
pip install -r requirements.txt
Or manually:
pip install langchainpip install langchain-communitypip install langchain-qdrantpip install langchain-huggingfacepip install sentence-transformerspip install qdrant-clientpip install python-dotenvpip install openaipip install pypdf

🔑 Environment Variables
Create a .env file:
QDRANT_API_KEY=your_qdrant_api_keyQDRANT_URL=your_qdrant_urlGROQ_API_KEY=your_groq_api_key

📚 Add Your PDF
Place your PDF inside project folder:
ramayan-eng.pdf

🧠 Index The PDF
Run:
python index.py
This will:


Load PDF


Split into chunks


Generate embeddings


Store vectors in Qdrant



💬 Start Chatbot
Run:
python chat.py
Example:
ask something => Who is Hanuman?

⚙️ Current Model
Embeddings
sentence-transformers/all-MiniLM-L6-v2
LLM
llama-3.3-70b-versatile
via Groq API.

📂 Project Structure
ramayan-ai/│├── index.py├── chat.py├── .env├── requirements.txt├── ramayan-eng.pdf└── README.md

🚀 Future Improvements


Streamlit/React frontend


Conversational memory


Multi-language support


Voice interaction


Hybrid search


Citation highlighting


Character-specific search


Sanskrit/Hindi support



📜 Example Queries
Describe Lord Rama's appearance
Who was Ravana?
Tell me about Hanuman's devotion
What happened during Sita Haran?

🧠 What is RAG?
RAG (Retrieval-Augmented Generation) retrieves relevant chunks from documents before sending them to the LLM, making responses:


more accurate


context-aware


cheaper


scalable


Instead of sending the entire PDF to the AI model every time.

🙌 Credits


Valmiki Ramayan


Project Gutenberg edition 


LangChain


Qdrant


HuggingFace


Groq



⭐ If You Like This Project
Give it a star on GitHub ⭐
