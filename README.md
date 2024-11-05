# Chat with PDF using RGemini
This Streamlit app lets you upload PDFs, process their text, and chat with the content by asking questions. It uses Google Gemini API for embeddings and conversational AI, storing processed data in a FAISS vector database
Requirements: Python 3.9+, Google Gemini API Key.
Installation: pip install streamlit PyPDF2 langchain langchain_google_genai google-generativeai faiss-cpu python-dotenv
GOOGLE_API_KEY=your_google_api_key_here
streamlit run app.py
## Interface:
Sidebar: Upload PDFs, then click Submit & Process to extract and save text chunks in FAISS.
Main Page: Enter questions based on the PDF content.
## Key Functions
1.get_pdf_text: Extracts text from PDFs.
2.get_text_chunks: Splits text into chunks.
3.get_vector_store: Saves text chunks in FAISS for search.
4.user_input: Handles user questions and provides answers based on PDF content.
