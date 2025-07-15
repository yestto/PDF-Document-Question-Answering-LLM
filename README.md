# PDF Query with LangChain and OpenAI

This project enables querying the contents of PDF documents using **LangChain**, **OpenAI's GPT**, and optionally **Astra DB** for vector storage and retrieval. It allows you to upload a PDF and ask natural language questions based on its content.

## 🚀 Features

- PDF text extraction
- Embedding generation using OpenAI
- Vector store support (e.g., Astra DB)
- Natural language querying using LangChain chains
- Environment variable-based secure key handling

## 📁 Files

- `PDFQuery_LangChain.ipynb`: Main Jupyter notebook for running the PDF query pipeline
- `requirements.txt`: Python package dependencies

## 🔧 Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yestto/PDFQuery_LangChain.git
   cd PDFQuery_LangChain
   ```

2. **Create and activate a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Create a `.env` file with the following content:**
   ```env
   ASTRA_DB_APPLICATION_TOKEN=AstraCS:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
   ASTRA_DB_ID=xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
   OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
   ```

5. **Run the notebook:**
   ```bash
   jupyter notebook PDFQuery_LangChain.ipynb
   ```

## 📚 Tech Stack

- [LangChain](https://github.com/hwchase17/langchain)
- [OpenAI GPT API](https://platform.openai.com/)
- [Astra DB (optional)](https://www.datastax.com/astra)
- `PyMuPDF` or `pdfminer.six` for PDF parsing
- Jupyter Notebook

