# PDF QnA Chatbot
A conversational chatbot that allows users to upload PDF documents and ask questions about their content. The bot built with Langchain, OpenAI's language models and leverages retrieval-augmented generation (RAG) to provide accurate, context-aware answers based on the content of the uploaded PDF.

## Technical Implementation
Document Loading: Handles PDF file ingestion using PyPDFLoader
Text Chunking: Splits documents into manageable chunks using RecursiveCharacterTextSplitter
Embeddings: Creates vector representations using OpenAIEmbeddings
Vector Store: Stores document chunks in DocArrayInMemorySearch for efficient retrieval
User Interface: Interactive dashboard utilizing python library (panel)

## Workflow
User uploads a PDF document
Document is processed, chunked, and stored in a vector database
User asks questions via the chat interface
System retrieves relevant document sections
GPT-3.5 generates contextual responses based on the retrieved information
User can view the conversation history and the sources of information