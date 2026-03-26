# YouTube RAG Application 📺🤖

The **YouTube RAG Application** is a powerful tool designed to interact with YouTube video content using Retrieval-Augmented Generation (RAG). By fetching transcripts directly from YouTube, the application enables users to ask detailed questions and receive accurate answers based on the video's content, effectively transforming any video into a searchable knowledge base.

## 🚀 Features

- **Automated Transcript Fetching**: Seamlessly retrieves video transcripts using the `youtube-transcript-api`.
- **Intelligent Text Chunking**: Utilizes `RecursiveCharacterTextSplitter` from LangChain to break down long transcripts into manageable, context-rich segments.
- **High-Performance Vector Storage**: Implements `FAISS` for rapid similarity searches across millions of vector embeddings.
- **State-of-the-Art Embeddings**: Leverages `HuggingFaceEmbeddings` for high-quality semantic representations of text.
- **Advanced Q&A Orchestration**: Powered by `LangChain` to provide a robust framework for RAG-based interactions.

## 🛠️ Project Structure

- `rag.ipynb`: The core Jupyter Notebook containing the full RAG pipeline, from fetching transcripts to querying the model.
- `main.py`: A placeholder entry point for future CLI integration.
- `requirements.txt`: Lists all the necessary Python libraries.
- `pyproject.toml` & `uv.lock`: Project configuration and dependency locking using `uv`.

## 📦 Tools & Technologies

| Tool | Purpose |
| :--- | :--- |
| **Python** | Core programming language |
| **LangChain** | RAG orchestration and chain development |
| **FAISS** | Fast vector library for similarity search |
| **Hugging Face** | Transformer-based embeddings |
| **YouTube Transcript API** | Fetches video captions/transcripts |
| **Wikipedia (optional)** | Used for augmenting context |

## ⚙️ Setup & Installation

### 1. Prerequisites
- Python 3.9 or higher
- `uv` (recommended) or `pip`

### 2. Create Virtual Environment
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configuration
Create a `.env` file in the root directory to store your API keys (e.g., Hugging Face Token):
```env
HUGGINGFACE_TOKEN=your_token_here
```

## 📖 Usage

1. Open the `rag.ipynb` notebook in VS Code or Jupyter.
2. Replace the `video_id` in the code cell with the ID of the YouTube video you want to analyze.
3. Run the cells sequentially to build the vector store and start asking questions!

---
*Created with ❤️ for exploring the future of AI-driven video interaction.*
