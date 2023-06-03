Chat with multiple PDFs
This project is a Streamlit web application that allows users to upload PDF files and interact with their content in a conversational manner. The application uses OpenAI's GPT model, FAISS, PyPDF2 and other tools to extract text from PDFs, generate vector representations, and answer questions about the content.

Setup
Clone the repository.
Create a Python virtual environment: python -m venv venv
Activate the virtual environment: .\venv\Scripts\activate.bat on Windows or source venv/bin/activate on Unix-based systems.
Install the dependencies: pip install -r requirements.txt
Run the Streamlit application: streamlit run app.py
Usage
After starting the application:

Upload one or more PDF files using the file uploader in the sidebar.
Click the "Upload" button to process the PDFs.
In the main panel, type a question about the content of the uploaded documents in the text input box and press enter.
The application will display a conversational exchange where the responses are generated based on the content of the uploaded documents.
Contributing
Please feel free to fork the repository and submit pull requests. For major changes, open an issue first to discuss what you would like to change.
