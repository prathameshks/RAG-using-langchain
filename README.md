# Complete RAG Implementation

This repository contains a complete implementation of a **Retrieval-Augmented Generation (RAG)** chatbot using **LangChain** and **ChromaDB**. The chatbot integrates cutting-edge technologies to deliver highly contextual and relevant responses based on a provided knowledge base.

---

## Features

- **Embedding with Hugging Face API**: Uses state-of-the-art models to generate embeddings for knowledge documents, ensuring accurate retrieval of relevant context.
- **ChromaDB as Vector Database**: Efficiently stores and queries document embeddings to enable fast and precise context retrieval.
- **Response Generation with Google AI Studio**: Generates human-like and context-aware responses using advanced AI models.
- **Seamless Query Relevance Check**: Incorporates logic to ensure queries are relevant to the knowledge base, enhancing response accuracy.

---

## Architecture

1. **Query Processing**:
   - User inputs a query.
   - Top relevant documents are retrieved using embeddings stored in ChromaDB.

2. **Prompt Construction**:
   - Context is extracted from retrieved documents.
   - A structured prompt is created and sent to the response generation model.

3. **Response Generation**:
   - Google AI Studio processes the prompt and generates a response.
   - The response is streamed or displayed to the user.

4. **Source Highlighting**:
   - Provides sources used to generate the response for transparency.

---

## Setup Instructions

### Prerequisites

1. Python 3.9+
2. Hugging Face API key
3. Google AI Studio API key
4. Required Python packages (listed in `requirements.txt`)

---

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/prathameshks/RAG-using-langchain.git
   cd RAG-using-langchain
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up API keys:
   - Add your Hugging Face and Google AI Studio keys to the `.env` file:
     ```
     HF_TOKEN=<your-huggingface-key>
     GOOGLE_API_KEY=<your-google-ai-key>
     ```

---

### Usage

1. Add PDFs to data folder.

2. Run the cells in the Jupyter notebook.

3. Provide Inputs where asked and Done.

---

This repository serves as a foundational implementation of RAG using LangChain and ChromaDB, with seamless integration of Hugging Face embeddings and Google AI Studio for response generation. 🚀