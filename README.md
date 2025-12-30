🔍 Project Overview

This project is a Streamlit-based chatbot that enables users to query information from their own PDF documents using natural language. The application extracts text from uploaded PDFs, splits the content into meaningful chunks, and converts them into vector embeddings stored in a FAISS index. When a user asks a question, the system retrieves the most relevant document segments and uses an OpenAI language model to generate accurate, context-aware answers. This solution simplifies document exploration and enhances productivity by eliminating manual searching.

⚙️ How It Works
User uploads a PDF file through the Streamlit interface.
Text is extracted from the PDF using PyPDF2.
The extracted text is split into overlapping chunks using RecursiveCharacterTextSplitter.
Each chunk is converted into embeddings using OpenAI Embeddings.
FAISS is used to store and perform similarity search on embeddings.
Relevant chunks are passed to an OpenAI Chat model to generate precise answers.

🧰 Tech Stack
Python
Streamlit – UI for file upload and chat interaction
LangChain – Text splitting, embeddings, and QA chain
FAISS – Vector database for similarity search
OpenAI API – Language model for generating responses
PyPDF2 – PDF text extraction

🚀 Features
Query custom PDF documents using natural language
Fast and efficient document search using vector embeddings
Clean and interactive Streamlit interface
Context-aware and accurate responses
No need for manual keyword searching
🛠️ Installation & Setup
pip install streamlit PyPDF2 langchain faiss-cpu openai

Set your OpenAI API key:

export OPENAI_API_KEY="your_api_key_here"

Run the application:

streamlit run app.py

📌 Use Cases

Research document analysis

Academic notes querying

Internal company document search

Personal knowledge base chatbot
