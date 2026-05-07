🕉️ Ramayan AI
An AI-powered RAG chatbot that lets you chat with the Ramayan using natural language.
Built using LangChain, Qdrant, HuggingFace embeddings, and Groq LLMs, the system retrieves relevant verses and passages from the Ramayan and generates contextual answers instead of sending the entire PDF to the AI model every time.

✨ Features


📖 Chat with the Ramayan conversationally


🔍 Semantic search using vector embeddings


🧠 RAG (Retrieval-Augmented Generation) architecture


⚡ Fast AI responses using Groq Llama models


🆓 Completely free local embeddings


🗂️ Qdrant vector database integration


📄 Multi-PDF support


🎯 Context-aware responses with source references


📚 Large PDF support (1900+ pages)



🏗️ How It Works
                 User Query                       ↓             Semantic Similarity Search                       ↓             Relevant Ramayan Chunks                       ↓                Context Injection                       ↓                  Groq LLM                       ↓                 Final Answer
Instead of sending the full Ramayan PDF to the AI model every time, only the most relevant chunks are retrieved and used for generating responses.
This makes the system:


faster


cheaper


scalable


more accurate



🧠 RAG Architecture
Ramayan PDF      ↓Text Chunking      ↓MiniLM Embeddings      ↓Qdrant Vector Database      ↓Semantic Retrieval      ↓Relevant Context      ↓Groq LLM      ↓AI Generated Response

🛠️ Tech Stack
TechnologyPurposePythonCore backendLangChainRAG orchestrationQdrantVector databaseHuggingFaceLocal embeddingsGroq APILLM inferencePyPDFLoaderPDF processing

📦 Installation
1. Clone Repository
git clone https://github.com/yourusername/ramayan-ai.gitcd ramayan-ai

2. Create Virtual Environment
python -m venv .venv
Activate Environment
Windows
.venv\Scripts\activate
Linux / Mac
source .venv/bin/activate

3. Install Dependencies
pip install -r requirements.txt
Or manually:
pip install langchainpip install langchain-communitypip install langchain-qdrantpip install langchain-huggingfacepip install sentence-transformerspip install qdrant-clientpip install python-dotenvpip install openaipip install pypdf

🔑 Environment Variables
Create a .env file in the root directory:
QDRANT_API_KEY=your_qdrant_api_keyQDRANT_URL=your_qdrant_urlGROQ_API_KEY=your_groq_api_key

📚 Add The Ramayan PDF
Place your PDF inside the project directory:
ramayan-eng.pdf

🧠 Index The PDF
Run:
python index.py
This process:


loads the PDF


splits it into chunks


creates embeddings


stores vectors in Qdrant



💬 Start The Chatbot
Run:
python chat.py
Example:
ask something => Who is Hanuman?
ask something => Describe Lord Rama's appearance
ask something => What happened during Sita Haran?

⚙️ Models Used
Embedding Model
sentence-transformers/all-MiniLM-L6-v2
LLM
llama-3.3-70b-versatile
via Groq API.

📂 Project Structure
ramayan-ai/│├── index.py├── chat.py├── requirements.txt├── .env├── ramayan-eng.pdf└── README.md

🚀 Future Improvements


🌐 Web interface (React / Streamlit)


🧠 Conversational memory


🎙️ Voice-based interaction


🌍 Hindi/Sanskrit support


📌 Citation highlighting


🔎 Character-specific search


📱 Mobile-friendly UI


🧬 Hybrid search (keyword + vector)



🧪 Example Queries
Who is Ravana?
Describe Hanuman's devotion to Rama
What is the story of Sita Haran?
Tell me about Lakshman's loyalty

🧠 What Is RAG?
RAG (Retrieval-Augmented Generation) is a technique where relevant information is first retrieved from documents before sending context to the AI model.
This allows the chatbot to:


answer based on actual documents


reduce hallucinations


improve accuracy


handle very large PDFs efficiently



🙌 Credits


Valmiki Ramayan


Project Gutenberg edition 


LangChain


Qdrant


HuggingFace


Groq



⭐ Support
If you liked this project, consider giving it a star on GitHub ⭐
