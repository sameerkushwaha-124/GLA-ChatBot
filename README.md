## Chat bot App Gla University
This project involves developing an interactive chatbot application using Streamlit, which integrates PDF processing capabilities and leverages Google Generative AI (Gemini Pro) for generating conversational responses. Here’s a detailed description of the project:

Project Description: GLA ChatBot Help & Support
Objective:
Create a chatbot that can help users by answering questions based on the content of uploaded PDF files. The application will process the PDFs, generate embeddings, and use a vector store for efficient text search and retrieval.

Key Components:

PDF Processing:

Use PyPDF2 to read and extract text from the uploaded PDF files.
Split the extracted text into manageable chunks using RecursiveCharacterTextSplitter to facilitate better processing and retrieval.
Embedding and Vector Store:

Generate embeddings for the text chunks using GoogleGenerativeAIEmbeddings.
Store the embeddings in a FAISS vector store to allow efficient similarity searches.
Conversational AI:

Implement a conversational chain using ChatGoogleGenerativeAI model (Gemini Pro) for generating detailed responses.
Create a custom prompt template to ensure accurate and context-specific responses.
User Interface:

Develop the frontend using Streamlit, providing a simple and interactive user interface.
Allow users to upload PDF files via a sidebar menu and ask questions through a text input field.
Display the chatbot's responses within the Streamlit app.
Workflow:

User uploads PDF files.
The application processes the PDFs, extracts text, and generates text chunks.
Embeddings are created for the text chunks and stored in a FAISS vector store.
When a user asks a question, the application searches for similar text chunks in the vector store.
The chatbot uses the retrieved text chunks to generate a response to the user's question.
