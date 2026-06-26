# Agentic RAG System

An **Agentic Retrieval-Augmented Generation (RAG)** system built using **LangGraph**, **LangChain**, **Google Gemini**, and **ChromaDB**. The agent intelligently decides whether to answer from uploaded documents, perform a web search, or respond using the LLM's general knowledge.

## Features

* Agentic workflow using **LangGraph**
* Dynamic PDF upload and indexing
* Retrieval-Augmented Generation (RAG)
* Real-time web search support
* General-purpose LLM responses
* Automatic tool selection based on the user query
* ChromaDB vector store with HuggingFace embeddings

## Tech Stack

* LangGraph
* LangChain
* Google Gemini
* ChromaDB
* HuggingFace Embeddings
* PyPDFLoader

## Workflow

1. Upload a PDF document.
2. The document is split, embedded, and stored in ChromaDB.
3. The agent analyzes the user query.
4. Based on the query, it chooses one of the following:

   * **RAG** – Retrieve information from the uploaded document.
   * **Web Search** – Fetch recent or real-time information.
   * **General LLM** – Answer using Gemini's knowledge.
5. The final response is returned to the user.

## Project Structure

```
├── Document Upload
├── Vector Store Creation
├── Tool Definitions
│   ├── RAG Tool
│   ├── Web Search Tool
│   └── General LLM Tool
├── LangGraph Agent
└── Interactive Query Interface
```

## Use Cases

* Document Question Answering
* Research Assistant
* Technical Documentation Search
* Educational PDF Chatbot
* Hybrid Knowledge Assistant

## Future Improvements

* Support multiple document collections
* Conversation memory
* Source citation and references
* Streaming responses
* Multi-modal document support

## License

This project is intended for learning and research purposes.
