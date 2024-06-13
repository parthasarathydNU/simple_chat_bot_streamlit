# Local LLM Chatbot

This project sets up a Streamlit-based chatbot that interacts with a locally hosted language model.

## Prerequisites

Make sure you have the following installed:
- Python 3.7+
- `pip`

## Installation

1. **Clone the repository**:

    ```bash
    git clone https://github.com/parthasarathydNU/simple_chat_bot_streamlit.git
    cd simple_chat_bot_streamlit
    ```

2. **Create a virtual environment**:

    ```bash
    python -m venv venv
    ```

3. **Activate the virtual environment**:

    - On Windows:

        ```bash
        .\venv\Scripts\activate
        ```

    - On macOS and Linux:

        ```bash
        source venv/bin/activate
        ```

4. **Install the required packages**:

    ```bash
    pip install -r requirements.txt
    ```

5. **Ensure your local language model service is running**:
    Follow the steps mentioned here to download a local instance of Ollama: `https://github.com/ollama/ollama?tab=readme-ov-file`

    Start your local instance of the LLM service (e.g., llama). Refer to the specific documentation of the service for setup instructions. Example command to start the service:

    ```bash
    ollama serve --model gemma:2b
    ```

## Running the Chatbot

1. **Start the Streamlit application**:

    ```bash
    streamlit run chatbot.py
    ```

2. **Open your web browser** and navigate to the URL provided by Streamlit (usually `http://localhost:8501`).

3. **Interact with the chatbot** by typing messages and receiving responses from the local LLM service.

## Project Structure

```
.
├── chatbot.py          # Main Streamlit application
└── requirements.txt    # Python dependencies
```

## Contributing

Feel free to submit issues and pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License.
