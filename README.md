# RAG Document Q&A on AWS Bedrock

A retrieval-augmented generation (RAG) application built to practice grounded question answering over documents. It answers questions about French and English PDFs using only the content it retrieves from them.

## Features

- **PDF ingestion:** French and English PDFs are chunked and embedded with a multilingual model.
- **Vector search:** the embeddings are stored in ChromaDB and the most relevant chunks are retrieved for each question.
- **Grounded answers:** Claude on AWS Bedrock (Converse API) answers only from the retrieved chunks.
- **Sources:** every answer comes with its source file and page.
- **API:** exposed through FastAPI.

## Tech stack

Python · FastAPI · ChromaDB · sentence-transformers · AWS Bedrock (Claude) · boto3 · pypdf
