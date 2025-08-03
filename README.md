# Langchain Demo with Gemma Model

This is a simple Streamlit application that demonstrates how to use the Gemma 2B model with LangChain and Ollama. Users can ask a question, and the application will display the model's response.

## Features

- **Framework**: Streamlit
- **LLM Integration**: LangChain with Ollama
- **Model**: Gemma 2B
- **Monitoring**: Langsmith

## Setup

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    ```

2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3.  **Install dependencies:**
    Make sure you have a `requirements.txt` file with the following content:
    ```
    langchain-ollama
    streamlit
    python-dotenv
    langchain
    ```
    Then run:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Create a `.env` file:**
    Create a file named `.env` in the root directory and add your Langsmith credentials:
    ```
    LANGCHAIN_API_KEY="your_langchain_api_key"
    LANGCHAIN_PROJECT="your_langchain_project_name"
    ```

## Running the Application

To run the app, execute the following command in your terminal:

```bash
streamlit run 1.2-ollama/app.py
```

## Usage

1.  Once the app is running, open your web browser and navigate to the local URL provided by Streamlit (e.g., `http://localhost:8501`).
2.  Type your question into the text input field.
3.  The model's answer will be displayed on the screen.
