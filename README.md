# GDrive RAG System

A Retrieval-Augmented Generation (RAG) system built with LangChain that allows you to chat with files stored in Google Drive. While the system supports Google Drive files in general, it is currently used to search and answer questions about my Google Docs notes.

## Features

- Connects to Google Drive as the knowledge source
- Loads and indexes supported files from Google Drive
- Detects document content changes using SHA-256 hashing and automatically rebuilds the vector store when updates are found
- Performs semantic search using vector embeddings
- Retrieves relevant context for user queries
- Generates context-aware responses with an LLM
- Implemented in a Jupyter Notebook for easy experimentation and development

## Tech Stack

- Python
- Jupyter Notebook
- LangChain
- Google Drive API
- Generative Model
- Embeddings Model (all-MiniLM-L6-v2)
- Vector Database (Chroma)

## Project Structure

```text
.
├── .credentials/
├── embeddings/
├── .env
├── .gitignore
├── document_hashes.json
├── gdrive_rag.ipynb
└── LICENSE.txt
└── README.md
```

## Installation

```bash
git clone <repository-url>
cd gdrive-rag-system
```

## Usage

1. Configure your Google Drive API credentials.
2. Set the required environment variables (LangSmith and Google API).
3. Run the notebook to index your Google Drive files.
4. On subsequent runs, the system compares each document's SHA-256 content hash with the previously stored hash.
5. If changes are detected, the vector store is rebuilt automatically before answering queries.

Example questions:

```text
What are the different vector search algorithms?
How do we optimize retrieval?
Where did I mention foundation models?
```

## Future Improvements

- Support for additional file types (pdf, sheets)
- Metadata filtering
- Web interface
- Conversation memory
- Incremental indexing

## License

This project is licensed under the MIT License.
