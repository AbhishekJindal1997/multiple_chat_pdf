# Chat with Multiple PDFs

This project is a Streamlit application that allows users to interact with multiple PDF documents. It uses the Langchain library to provide a conversational interface for asking questions about the contents of the uploaded PDFs.

## How it works

The application works in several steps:

1. **PDF Upload:** Users can upload one or more PDF documents via the sidebar.
2. **PDF Processing:** The text is extracted from each page of each uploaded PDF.
3. **Text Splitting:** The raw text from the PDFs is split into chunks using a character-based text splitter from the Langchain library.
4. **Vector Store Creation:** A vector store is created from the text chunks using OpenAI embeddings. This vector store is used for retrieving relevant information in response to user queries.
5. **Conversation Chain Creation:** A conversation chain is created, which uses a ChatOpenAI model, a FAISS retriever (created from the vector store), and a conversation buffer memory. This conversation chain is used to handle user queries.

## Usage

To use the application:

1. Clone this repository.
2. Install the required Python packages (listed in `requirements.txt`).
3. Run the Streamlit application with `streamlit run app.py`.
4. Upload one or more PDFs via the sidebar.
5. Ask a question about the documents in the main text input field.

## Note

This project is an example of how to use the Langchain library for document retrieval. It should be adapted to your specific use case and requirements.
