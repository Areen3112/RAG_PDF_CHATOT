# 📄 RAG PDF Chatbot

An intelligent **Retrieval-Augmented Generation (RAG) PDF Chatbot** built using **Streamlit** and **LangChain** that enables users to upload PDF documents and ask questions based on their content. The application retrieves relevant information from the uploaded document and generates context-aware responses using Large Language Models (LLMs).

## 🚀 Features

- 📂 Upload and process PDF documents through a user-friendly interface.
- 💬 Ask natural language questions related to the uploaded PDF.
- 🔍 Retrieves the most relevant document sections before generating responses.
- 🧠 Uses the **RAG (Retrieval-Augmented Generation)** approach for accurate, document-grounded answers.
- ⚡ Simple implementation with a single `app.py` file.
- 🎨 Interactive web interface powered by Streamlit.

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|-----------|
| **Python** | Core programming language |
| **Streamlit** | Web application framework |
| **LangChain** | RAG pipeline orchestration |
| **PDF Processing Libraries** | Extract text from PDF files |
| **Embeddings Model** | Convert text chunks into vector representations |
| **Vector Store** | Store and retrieve relevant document chunks |
| **LLM** | Generate answers based on retrieved context |

---

## 📁 Project Structure

```text
rag-pdf-chatbot/
│
├── app.py            # Main application containing the complete RAG workflow
├── requirements.txt  # Project dependencies
└── README.md         # Project documentation
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Areen3112/rag-pdf-chatbot.git
cd rag-pdf-chatbot
```

### 2. Create a Virtual Environment (Recommended)

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

#### macOS/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

Launch the Streamlit app using:

```bash
streamlit run app.py
```

Once started, open your browser and navigate to:

```text
http://localhost:8501
```

---

## 📖 How It Works

### 1. Upload a PDF Document

Users upload a PDF file through the Streamlit interface.

### 2. Text Extraction

The application extracts textual content from the uploaded PDF.

### 3. Document Chunking

The extracted text is split into smaller chunks to improve retrieval performance.

### 4. Embedding Generation

Each chunk is converted into vector embeddings using an embedding model.

### 5. Vector Storage

The embeddings are stored in a vector database for efficient similarity search.

### 6. Query Processing

When a user asks a question:

- The query is converted into embeddings.
- Relevant document chunks are retrieved from the vector store.
- Retrieved context is sent to the LLM.
- The LLM generates an answer grounded in the PDF content.

---

## 🔄 RAG Workflow

```text
User Uploads PDF
        │
        ▼
Text Extraction
        │
        ▼
Text Chunking
        │
        ▼
Embedding Generation
        │
        ▼
Vector Store Creation
        │
        ▼
User Question
        │
        ▼
Similarity Search
        │
        ▼
Retrieve Relevant Chunks
        │
        ▼
LLM Generates Response
        │
        ▼
Answer Displayed to User
```

---

## 💡 Example Questions

After uploading a PDF, users can ask questions such as:

```text
"What are the main findings of this research paper?"
```

```text
"Summarize the methodology section."
```

```text
"Who are the authors of this document?"
```

```text
"What are the key conclusions mentioned in the report?"
```

```text
"Explain this topic in simple terms."
```

---

## 🎯 Use Cases

- 📚 Research Paper Assistant
- 🏢 Company Policy Document Chatbot
- ⚖️ Legal Document Exploration
- 📖 Educational Study Companion
- 📑 Technical Documentation Assistant
- 🧠 Personal Knowledge Base

---

## 🔮 Future Enhancements

- [ ] Support for multiple PDF uploads
- [ ] Chat history and conversational memory
- [ ] Source citations for generated answers
- [ ] Support for additional document formats (DOCX, TXT)
- [ ] Authentication and user sessions
- [ ] Improved UI/UX design
- [ ] Deployment on Streamlit Cloud
- [ ] Export chat conversations

---

## 🤝 Contributing

Contributions are welcome!

### Steps to Contribute

1. Fork the repository.

2. Create a feature branch:

```bash
git checkout -b feature/feature-name
```

3. Commit your changes:

```bash
git commit -m "Add some feature"
```

4. Push to the branch:

```bash
git push origin feature/feature-name
```

5. Open a Pull Request.

---

## 📋 Requirements

Typical dependencies used in this project include:

```text
streamlit
langchain
langchain-community
langchain-openai
pypdf
faiss-cpu
python-dotenv
openai
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

---

## 📜 License

This project is licensed under the **MIT License**.

You are free to use, modify, and distribute this software for educational and commercial purposes.

---

## 👨‍💻 Author

### Areen Joshi

- GitHub: `https://github.com/Areen3112`
- LinkedIn: `https://linkedin.com/in/areen-joshi`

If you found this project useful, please consider giving it a ⭐ on GitHub.

---

<div align="center">

### ⭐ Star this repository if you found it helpful!

**Built with Streamlit, LangChain, and the power of Retrieval-Augmented Generation (RAG).**

</div>
