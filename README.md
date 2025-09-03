# Therapeutic Chatbot

This project is an empathetic and supportive therapeutic chatbot. It leverages a powerful Retrieval-Augmented Generation (RAG) pipeline, combining the conversational abilities of the Gemini API with real-time web search results from DuckDuckGo. The chatbot's core purpose is to validate emotions and offer thoughtful, up-to-date advice, acting as a supportive personal assistant for managing stress and anxiety.

## Key Features

**Empathetic Persona**: Engineered to act as a psychological assistant, providing kind and caring responses.

**Real-Time Information**: Utilizes DuckDuckGo Search to fetch current data, ensuring its advice is relevant and grounded.

**Gemini API Integration**: Built on the powerful Gemini 1.5 Flash model for advanced reasoning and high-quality conversational output.

**Modular Architecture**: Separates the backend logic (backend.py) from the frontend interface (app.py) for clean, organized code.

**Streamlit Frontend**: A simple and user-friendly web interface for smooth interaction.
 
## How It Works

The chatbot uses a RAG pipeline to provide informed responses:

- Retrieve: When a user asks a question, the system searches relevant, real-time information from DuckDuckGo.

- Augment: The retrieved text is combined with the user's original query.

- Generate: The Gemini model uses this combined input to produce a precise, empathetic, and context-aware answer.

## Getting Started

Follow these steps to set up and run the project on your local machine.

- Prerequisites
Python 3.8 or higher

A Gemini API Key. You can obtain one from the Google AI Studio or the Google Cloud Console.

- Installation
Clone this repository to your local machine:

git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
cd your-repository-name

- Install the required Python packages:

pip install -r requirements.txt

(If you don't have a requirements.txt file, you can generate one after installing the necessary packages: google-generativeai, duckduckgo-search, and streamlit.)

## Configuration

- Create a file named .env in your project's root directory.

- Add your Gemini API key to this file in the following format:

- GOOGLE_API_KEY="your_api_key_here"

- Replace "your_api_key_here" with your actual API key.

## Running the Application
Run the Streamlit application from your terminal:

streamlit run app.py

The application will open in your web browser, and you can begin interacting with the chatbot.

## File Structure
app.py: The Streamlit frontend code, handling the user interface and displaying responses.

backend.py: The core logic, including the RAG pipeline, API calls, and data retrieval.

.env: A hidden file for securely storing your API key.

requirements.txt: (Optional) Lists all the required Python libraries.

## Technologies Used
- Python: The core programming language.

- Google Gemini API: For generating empathetic and context-aware responses.

- Streamlit: For building the interactive web application.

- DuckDuckGo Search: Used as the real-time data source for the RAG pipeline.

- python-dotenv: For loading environment variables.

- functools.lru_cache: For caching search results to improve performance.

## License
This project is open-source.
