

# AI-Powered Conversational System for Multi-PDF Interaction

Overview

This project is an AI-powered conversational system designed to interact with multiple PDF documents. The system enables efficient querying and extraction of information from multiple PDFs, streamlining the process of document review and synthesis for users in various fields like research, law, and business.

The system integrates:

    LangChain for managing and processing large documents.
    Google Gemini Pro for advanced natural language understanding and question-answering.
    Streamlit for a user-friendly web interface to upload PDFs and ask questions.
    PyPDF2 for text extraction from PDF documents.
    FAISS (Facebook AI Similarity Search) for similarity-based text chunk retrieval.

Features

    Multi-PDF Management: Upload and interact with multiple PDF files simultaneously.
    Contextual Question Answering: Ask multi-part or follow-up questions and get relevant answers from various sources.
    Efficient Information Retrieval: Use chunk-based searching to improve response accuracy.
    User-Friendly Interface: A simple web-based interface for easy interaction.
    Scalable and Adaptable: Suitable for different fields, including legal case preparation, academic research, and business analytics.


Technologies Used

    LangChain: Manages text processing and question-answering capabilities.
    Google Gemini Pro: Interprets user queries and provides context-aware answers.
    PyPDF2: Extracts text from PDF documents for processing.
    FAISS: Provides efficient text similarity searching.
    Streamlit: A web framework for building the user interface.
    Python: Core language for implementing the system.

System Architecture

The system works by:

    Uploading PDFs: Users upload one or more PDF files via the web interface.
    Text Extraction: PyPDF2 extracts the content of the PDFs.
    Chunking & Indexing: LangChain splits the text into manageable chunks and FAISS creates a vector index for fast similarity searches.
    Embedding Generation: Google Gemini generates embeddings for the text chunks.
    Question Answering: Users input their questions, and the system finds relevant text chunks using FAISS and generates a response using Google Gemini's model.
    Display Results: The results are displayed in the Streamlit interface for easy viewing.

Installation

    Clone the repository:

    bash

git clone https://github.com/your-username/ai-conversational-pdf-system.git
cd ai-conversational-pdf-system

Install the required dependencies:

bash

pip install -r requirements.txt

Set up API keys:

    Obtain your Google API key for Google Gemini Pro.
    Create a .env file in the root of the project and add your API key:

    bash

    GOOGLE_API_KEY=your_api_key_here

Run the Streamlit app:

bash

    streamlit run app.py

    Upload PDFs and interact: Use the sidebar to upload PDF documents and start querying through the interface.

Usage

    Upload multiple PDFs using the Streamlit interface.
    Type in your question in the input field.
    Get context-aware answers from the system based on the content of your PDFs.

Example Queries

    "Summarize the main ideas from all PDFs."
    "What does Document A say about financial education?"
    "Compare the opinions on investment strategies from the uploaded PDFs."

Contributing

Feel free to fork this repository and contribute by submitting a pull request. Any contributions, whether it's improving functionality, documentation, or testing, are welcome!


Contact

For any questions or feedback, please reach out to me at [suryathirupks@gmail.com].
