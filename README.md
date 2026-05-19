# Healthcare RAG Assistant

Healthcare RAG Assistant is a Retrieval-Augmented Generation (RAG) web application designed to answer healthcare-related questions based on uploaded medical PDF documents. The system retrieves the most relevant document chunks and generates clear answers using a language model.

## Live Demo

[Open the Streamlit App](https://healthcare-rag-app-5fsqspsdgc7qdknpy3ng3x.streamlit.app/)

## Topics Covered

- Acne
- Eczema
- Psoriasis
- Skin Cancer

## Technologies Used

- Python
- Streamlit
- Sentence Transformers
- FAISS
- DeepSeek API
- PyPDF

## How It Works

1. The system reads medical PDF documents.
2. The text is split into smaller chunks.
3. Each chunk is converted into embeddings using `sentence-transformers/all-MiniLM-L6-v2`.
4. The embeddings are normalized and stored in a FAISS vector index.
5. When the user asks a question, the system retrieves the most relevant chunks.
6. The retrieved context is passed to DeepSeek to generate a clear and concise answer.

## Disclaimer

This application provides educational healthcare information only. It does not diagnose medical conditions and does not replace professional medical advice.
