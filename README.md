# Local-Restaurant-Recommendation-RAG

A fully local Retrieval-Augmented Generation (RAG) application that answers questions based on a dataset of restaurant reviews. This project ensures 100% data privacy by running the LLM, embedding model, and vector database entirely on your local machine without any cloud API calls.

## Features
* **Local AI Execution:** Uses Ollama to run Llama 3.2 locally.
* **Vector Search:** Converts restaurant reviews into mathematical embeddings and searches for the most relevant context using ChromaDB.
* **Interactive Chat:** An infinite loop terminal interface to ask questions about the restaurants in the dataset.
* **Data Ingestion:** Automatically reads reviews from a CSV file and populates the vector database on the first run.

## Tech Stack
* **Framework:** LangChain
* **LLM:** Ollama (Llama 3.2)
* **Embeddings:** Ollama (mxbai-embed-large)
* **Vector Database:** ChromaDB
* **Data Processing:** Pandas

## Prerequisites
Before running this project, you need to have Ollama installed on your machine and the specific models downloaded.

1. Install [Ollama](https://ollama.com/).
2. Open your terminal and pull the required models:
   ```bash
   ollama pull llama3.2
   ollama pull mxbai-embed-large
