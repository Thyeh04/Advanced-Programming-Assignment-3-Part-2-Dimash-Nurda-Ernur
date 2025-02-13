# Title  AI Assistant for Kazakhstan Constitution
This project provides an AI assistant that can answer questions about the Constitution of Kazakhstan. It uses Ollama LLM for generating responses and ChromaDB for storing and retrieving relevant context from uploaded PDF documents.

## Usage

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/shyr1es/Advanced-Programming-Assignment-3-Part-1-Dimash-Nurda-Ernur.git](https://www.google.com/search?q=https://github.com/shyr1es/Advanced-Programming-Assignment-3-Part-1-Dimash-Nurda-Ernur.git)
    cd Advanced-Programming-Assignment-3-Part-1-Dimash-Nurda-Ernur
    ```

2.  **Install dependencies:**

    ```bash
    pip install -r 
    ```

3.  **Start Ollama LLM:**

    Make sure you have Ollama LLM running locally.  The application connects to it at `http://localhost:11434`.  Refer to the Ollama documentation for installation and running instructions.  You'll need to download the `llama3.2` model (or whichever model you specify in `app.py`).

4.  **Run the Streamlit app:**

    ```bash
    streamlit run src/app.py
    ```

5.  **Upload PDF:** Open the Streamlit app in your browser. Upload the PDF file(s) of the Kazakhstan Constitution.

6.  **Ask a question:** Enter your question in the text input field and click "Submit."

7.  **View the answer:** The AI's response will be displayed below the input field.

8.  **View chat history:** Click the "Show Chat History" button to see the history of your queries and the AI's responses.

## Demo Screenshots

![image](https://github.com/user-attachments/assets/28ff3851-30b9-4fe5-94ab-82aee8f9dac4)
![image](https://github.com/user-attachments/assets/8cc7a864-22da-4cba-9bfb-1d6e30df3fa7)
![image](https://github.com/user-attachments/assets/5c7a3a9b-11a8-42bf-babb-b67d263ddfe2)
![image](https://github.com/user-attachments/assets/73b3f824-380b-4aae-b71b-6d5a05aaaca2)



## Examples

**Example 1: Uploading a PDF**

1.  Click the "Browse files" button in the Streamlit app.
2.  Select the PDF file of the Kazakhstan Constitution.
3.  The app will process the PDF and store the text in ChromaDB.  You'll see a success message and a preview of the extracted text.

**Example 2: Asking a question**

1.  Enter your question in the text input field (e.g., "What are the fundamental principles of the Constitution?").
2.  Click the "Submit" button.
3.  The app will retrieve relevant context from ChromaDB, send the question and context to Ollama LLM, and display the AI's response.

**Example 3: Viewing chat history**

1.  Click the "Show Chat History" button.
2.  The app will display a list of previous questions and answers.

**Example 4: No relevant context**

1. Upload a PDF.
2. Ask a question that is not related to the content of the PDF.
3. The app will warn you that no relevant context was found and will use only your question to query the LLM.

**Example 5: Error handling**

1. If Ollama is not running, the app will display an error message.
2. If there is an issue reading the PDF, the app will display an error message.
