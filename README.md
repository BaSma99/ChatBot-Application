# Google AI Text Generation Chatbot

## Overview

This project implements a chatbot using Streamlit and Google Generative AI (Gemini Pro). The chatbot generates text responses based on user input by utilizing Google's generative AI capabilities.

## Requirements

- Python 3.x
- `streamlit` library
- `google-generativeai` library

## Installation

1. Clone or download this repository.
2. Install the required dependencies:

```bash
pip install streamlit google-generativeai
```

## Setup

### Google API Key

You need a valid Google API key for authentication to use the Google Generative AI API. You can obtain an API key from [Google Cloud](https://cloud.google.com/).

### Configuration

In the `chatBot.py` file, replace the API key in the `api` variable with your own key:

```python
api = 'YOUR_GOOGLE_API_KEY'
```

## Running the Chatbot

1. After setting up the required dependencies and API key, run the Streamlit app:

```bash
streamlit run chatBot.py
```

2. The app will launch in your web browser, where you can interact with the chatbot.

## How It Works

- The app uses Streamlit to create an interactive user interface.
- When the user inputs a message, it is sent to the Google Generative AI model (Gemini Pro) for content generation.
- The generated response is displayed back to the user.
- The interaction is logged in the session state, ensuring a smooth conversation flow between the user and the assistant.

## Functions

- `Generate_Text(text)`: This function sends the user's input to the Google Generative AI model (`gemini-pro`) and retrieves a generated response.

## Notes

- The app maintains a chat session, so users can interact with the assistant in a continuous manner.
- If the API key is invalid, the app will display an error message.
  
