# GDrive RAG System

A Retrieval-Augmented Generation (RAG) system built with LangChain that allows you to chat with files stored in Google Drive. While the system supports Google Drive files in general, it is currently used to search and answer questions about my Google Docs notes.

## Features

- Connects to Google Drive as the knowledge source
- Loads and indexes supported files from Google Drive
- Performs semantic search using vector embeddings
- Retrieves relevant context for user queries
- Generates context-aware responses with an LLM
- Implemented in a Jupyter Notebook for easy experimentation and development

## Tech Stack

- Python
- Jupyter Notebook
- LangChain
- Google Drive API
- Generative Model (Gemini 2.5 Flash)
- Embeddings Model (all-MiniLM-L6-v2)
- Vector Database (Chroma)

## Project Structure

```text
.
├── .credentials/
├── chroma_langchain_db/
├── .env
├── .gitignore
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
2. Set the required environment variables (Langsmith and Google API).
3. Index your Google Drive files.
4. Start querying your documents.

Example questions:

```text
What are the different vector search algorithms?
How do we optimize retrieval?
Where did I mention foundation models?
```

## Future Improvements

- Automatic synchronization with Google Drive
- Support for additional file types
- Metadata filtering
- Web interface
- Conversation memory
- Incremental indexing

## License

This project is licensed under the MIT License.
