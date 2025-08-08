# RAG-based AI Chatbot with Gemini API and Qdrant Vector Store

This project demonstrates a **Retrieval-Augmented Generation (RAG)** pipeline built with:
- **[Gemini API](https://ai.google.dev/gemini-api)** for powerful natural language understanding and generation.
- **[Qdrant](https://qdrant.tech/)** as a high-performance vector database for semantic search and retrieval.

The goal is to combine the generative capabilities of large language models with the precision of vector search, enabling the chatbot to answer questions based on custom knowledge sources.

---

## 🚀 Features
- **Custom Knowledge Base**: Store and search your own documents in Qdrant.
- **Semantic Retrieval**: Use embeddings to find the most relevant chunks of information.
- **Gemini-powered Responses**: Generate rich, context-aware answers using the retrieved data.
- **Modular Architecture**: Easy to extend with new data sources or APIs.
- **Fast & Scalable**: Qdrant ensures low-latency search even with large datasets.

---

## 🛠 Tech Stack
- **Backend**: Python 3.x
- **LLM API**: Google Gemini API
- **Vector Store**: Qdrant
- **Embeddings**: Gemini embeddings or alternative embedding models
- **Data Processing**: LangChain / Custom pipeline (depending on your implementation)

---

## 📦 Installation

1. **Clone this repository**:
```bash
   git clone https://github.com/yourusername/rag-gemini-qdrant.git
   cd rag-gemini-qdrant
```
2. **Create a virtual environment:**
```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. **Install:**
```bash
pip install -r requirements.txt
```
4. **Build:**
```bash
docker compose up --build
```
## Usage
1. From your web browser, type http://localhost:8501 .
2. A web page will show, there's an input box where you can enter your question.
3. Press Enter, the system will get the answer and show below the header "Answer"
4. You can also go to http://localhost:8000/docs to test the APIs
5. The notebook used to divide the pdf into chunks, get embeddings, and populate Qdrant database is `Rag_Data/qa_data_prep.ipynb`