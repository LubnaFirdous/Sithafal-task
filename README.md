# Chat with PDF using RAG (Retrieval-Augmented Generation)

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline using `LangChain`, `FAISS`, `SentenceTransformers`, and `OpenAI GPT` to enable conversational querying of information from PDF files.

With this application, you can:
- Upload one or more PDF files.
- Ask questions about the contents of the uploaded PDFs.
- Get relevant responses powered by embeddings and GPT.

---

## **Features**
- **PDF Processing**: Extracts text from PDF files using `pdfplumber`.
- **Chunking**: Splits text into manageable chunks for efficient processing.
- **Embeddings**: Generates vector embeddings using `SentenceTransformers`.
- **FAISS Indexing**: Enables fast similarity searches on the embedded text.
- **OpenAI Integration**: Generates answers to user queries based on the retrieved text chunks.

---

## **How It Works**
1. **Upload PDFs**: Upload one or more PDF files via the Streamlit interface.
2. **Text Extraction**: Extracts text from the uploaded PDF files.
3. **Text Chunking**: Splits the extracted text into smaller chunks for better search accuracy.
4. **Embedding Generation**: Converts text chunks into vector embeddings using a pre-trained model.
5. **FAISS Search**: Uses FAISS to find the most relevant chunks for a user's query.
6. **OpenAI GPT**: Combines the retrieved text chunks into a context and generates answers using OpenAI GPT.

---

## **Technologies Used**
- **[Streamlit](https://streamlit.io/)**: For the web interface.
- **[pdfplumber](https://github.com/jsvine/pdfplumber)**: To extract text from PDF files.
- **[SentenceTransformers](https://www.sbert.net/)**: To generate embeddings for text.
- **[FAISS](https://github.com/facebookresearch/faiss)**: For similarity search.
- **[LangChain](https://langchain.readthedocs.io/)**: For text processing and prompt handling.
- **[OpenAI API](https://platform.openai.com/)**: To generate answers using GPT models.

---

## **Setup Instructions**
Follow these steps to set up and run the project locally:

### 1. **Clone the Repository**
```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
