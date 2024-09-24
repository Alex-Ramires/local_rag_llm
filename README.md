# Shrek Scripts Q&A with Llama 3.1 (RAG-based)

This project demonstrates how to apply Retrieval-Augmented Generation (RAG) using the Llama 3.1 model to answer questions based on the movie scripts of **Shrek 1** and **Shrek 2**. Specifically, it uses the **Ollama** Llama3.1 model to process the documents and answer questions like _"What is the effect of the Happily Ever After Potion?"_.

The workflow involves loading the scripts in PDF format, chunking them into smaller parts, and creating embeddings to build a vector database. Using the RAG technique, the system retrieves the most relevant chunks from the scripts and generates answers using Llama 3.1.

### Install Ollama

Ollama is used to run the Llama 3.1 model locally. Follow the instructions to install it:

1. Visit [Ollama's website](https://ollama.com/) and follow the installation instructions for your OS.
2. Once installed, pull the required models:

```bash
ollama pull llama3.1
ollama pull nomic-embed-text
