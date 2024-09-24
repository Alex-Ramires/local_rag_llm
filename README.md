# Shrek Scripts Q&A with Llama 3.1 (RAG-based)

This project demonstrates how to apply Retrieval-Augmented Generation (RAG) using the Llama 3.1 model to answer questions based on the movie scripts of **Shrek 1** and **Shrek 2**. 

The workflow involves loading the scripts in PDF format, chunking them into smaller parts, and creating embeddings to build a vector database. Using the RAG technique, the system retrieves the most relevant chunks and generates answers based on the context.

### Step 1: Install Ollama

Ollama is used to run the Llama 3.1 model locally. Follow the instructions to install it:

1. Visit [Ollama's website](https://ollama.com/) and follow the installation instructions for your OS.
2. Once installed, pull the required models:

```bash
ollama pull llama3.1
ollama pull nomic-embed-text
```

### Step 2: Clone the Repository

```bash
git clone https://github.com/Alex-Ramires/local_rag_llm.git
cd local_rag_llm
```

### Step 3: Install the Python Dependencies

```bash
pip install -r requirements.txt
```
### Step 4: Run the jupyter notebook "1.0-rag-chain"

By default, the system will answer the question:

_What is the effect of the Happily Ever After Potion?_

The response will be printed in the console.

