# InsightBot

## Overview

RAG-PDF-Convo-Bot is a chatbot that allows users to upload a PDF document and interact with it conversationally. The bot is built using the LangChain framework and is powered by Retrieval-Augmented Generation (RAG) for efficient information retrieval. The chatbot is capable of answering questions related to the content of the uploaded PDF in English, while also keeping track of the conversation history through session IDs to remember follow-up questions.

## Features

- **PDF Upload & Chat:** Users can upload a PDF document and ask questions related to its content. The chatbot provides responses based on the information extracted from the PDF.
- **RAG-Powered Retrieval:** The chatbot leverages RAG to create chunks of text from the PDF and retrieve relevant information based on user queries.
- **Embeddings Generation:** Hugging Face's `all-MiniLM-L6-v2` model is used to generate embeddings for the PDF chunks, ensuring accurate semantic search.
- **Chroma DB Integration:** The embeddings generated from the PDF content are stored in Chroma DB, a vector database, which facilitates efficient retrieval of relevant chunks during the conversation.
- **Session-based Interaction:** The bot maintains a history of the conversation in the form of session IDs, enabling it to remember the context and follow-up questions within the same session.
- **Groq API:** The chatbot is integrated with the Groq API, utilizing the Gemma 2 model (9 billion parameters) for generating responses to user queries.
- **Streamlit Interface:** The entire application is deployed using Streamlit, providing an easy-to-use web interface for interacting with the chatbot.

## Tech Stack

- **LangChain:** A framework for building language model applications, used for managing the chatbot's conversation flow and integrating various components.
- **RAG (Retrieval-Augmented Generation):** A technique used to enhance the chatbot's information retrieval capabilities by breaking the PDF content into chunks and retrieving relevant information based on user queries.
- **Hugging Face's all-MiniLM-L6-v2:** A pre-trained model used for generating embeddings from the PDF content, allowing the chatbot to understand and retrieve semantically relevant information.
- **Chroma DB:** A vector database used to store and manage the embeddings generated from the PDF, enabling fast and accurate retrieval during conversations.
- **Groq API & Gemma 2 Model:** The Groq API is used to interact with the Gemma 2 language model, which powers the chatbot's response generation.
- **Streamlit:** A Python framework used to create a user-friendly web interface for the chatbot, allowing users to upload PDFs and chat with the bot easily.

## Usage
1. **Add Groq api key:** Enter groq api key, you can get it my signing up in groq cloud
1. **Upload PDF:** After that, upload a PDF document using the interface provided.
2. **Ask Questions:** Start asking questions related to the content of the uploaded PDF. The chatbot will respond based on the information extracted from the document.
3. **Session ID:** Each conversation is assigned a unique session ID. If you need to refer back to a previous conversation or continue the discussion, use the session ID to maintain context.
4. **Follow-up Questions:** The bot can remember the context of the conversation within the same session, allowing for follow-up questions without losing context. You can see whole chat history too.
## How to run?
Simply go to https://insightbot-3x71.onrender.com and use as started above. Yes it's that simple 😊

## Contributing

Contributions are welcome! Just drop an E-Mail at msinghmayank62@gmail.com




