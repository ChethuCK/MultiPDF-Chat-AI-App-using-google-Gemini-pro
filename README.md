# MultiPDF Chat AI App using Google Gemini Pro

## Overview
MultiPDF Chat AI App is a Streamlit-based application that enables users to interact with multiple PDF files using Google Gemini Pro AI. The app extracts text from PDFs, processes it using FAISS for efficient similarity search, and generates AI-driven responses based on user queries.

## Features
- Upload multiple PDF files.
- Extract and process text using `PyPDF2`.
- Chunk text for efficient retrieval using `langchain.text_splitter`.
- Store and retrieve text embeddings using FAISS.
- Utilize Google Gemini Pro AI for intelligent responses.
- Simple and intuitive UI built with Streamlit.

## Installation

### Prerequisites
Ensure you have Python installed on your system. Recommended version: Python 3.8+

### Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/multipdf-chat-ai.git
   cd multipdf-chat-ai
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows use `env\Scripts\activate`
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up your Google API key:
   - Create a `.env` file in the root directory.
   - Add the following line:
     ```
     GOOGLE_API_KEY=your_google_api_key_here
     ```

## Usage
1. Run the application:
   ```bash
   streamlit run app.py
   ```
2. Upload your PDF files using the sidebar.
3. Click "Submit & Process" to process the files.
4. Ask questions in the text input box, and the AI will provide relevant answers.

## Project Structure
```
MultiPDF-Chat-AI/
│── app.py                 # Main Streamlit application
│── requirements.txt       # Required dependencies
│── .env                   # Environment variables (API keys)
│── README.md              # Project documentation
```

## Dependencies
- `streamlit`
- `PyPDF2`
- `langchain`
- `FAISS`
- `google-generativeai`
- `python-dotenv`

## Acknowledgements
This project utilizes Google Gemini Pro AI and FAISS for document retrieval and conversational AI. Special thanks to the open-source community for their valuable contributions.

## License
This project is licensed under the MIT License. Feel free to modify and distribute it as per the license terms.

---

### Future Enhancements
- Add support for other document formats (Word, TXT, etc.).
- Implement session-based chat history.
- Enhance UI with more interactive elements.

