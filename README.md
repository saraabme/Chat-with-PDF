# Chat-with-PDF
Python application that allows you to upload a PDF and ask questions about it using natural language. The application uses a LLM to generate a response about your PDF. The LLM will not answer questions unrelated to the document.

## How it works
This application processes PDFs by breaking down the text into smaller segments, or chunks, suitable for input into a Large Language Model (LLM). It leverages OpenAI embeddings to convert these text segments into vector representations. When a user asks a question, the application identifies the text segments that are most semantically similar to the query and sends them to the LLM to generate a response. The LLM is designed to only answer questions related to the content of the document and will not respond to unrelated queries.

The application uses Streamlit to create the GUI and Langchain to deal with the LLM.

## Usage
Clone this repository and install the necessary requirements:

```pip install -r requirements.txt```


To use the application, run the main.py file with the streamlit CLI: 

```streamlit run app.py```
