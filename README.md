Therapeutic Chatbot
This project is a therapeutic chatbot designed to provide empathetic and supportive conversational assistance. It utilizes a powerful combination of the Gemini API for natural language generation and DuckDuckGo Search for real-time, context-aware information retrieval through a Retrieval-Augmented Generation (RAG) pipeline.

The chatbot is built with a caring and empathetic persona to validate emotions and offer thoughtful advice, making it a supportive personal assistant for managing stress and anxiety.

Features
Empathetic Persona: The chatbot is engineered to act as a psychological assistant, providing kind and supportive responses.

Real-Time Information (RAG): It retrieves and processes up-to-date information from the web using DuckDuckGo Search to ensure its advice is relevant and grounded.

Gemini API Integration: Leverages the Gemini 1.5 Flash model for advanced reasoning and high-quality conversational output.

Modular Architecture: Separates backend logic (backend.py) from the frontend interface (app.py) for clean, organized code.

Streamlit Frontend: Provides a simple and user-friendly web interface for interaction.

Getting Started
Follow these steps to set up and run the project on your local machine.

Prerequisites
Python 3.8 or higher

A Gemini API Key. You can obtain one from the Google AI Studio or the Google Cloud Console.

Installation
Clone this repository to your local machine.

git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
cd your-repository-name

Install the required Python packages.

pip install -r requirements.txt

(Note: If you don't have a requirements.txt file, create one by running pip freeze > requirements.txt after installing the packages mentioned in your code, which are google-generativeai, duckduckgo-search, and streamlit.)

Configuration
Create a file named .env in your project's root directory.

Add your Gemini API key to this file in the following format:

GOOGLE_API_KEY="your_api_key_here"

Replace "your_api_key_here" with your actual API key.

Running the Application
Run the Streamlit application from your terminal:

streamlit run app.py

The application will open in your web browser, and you can begin interacting with the chatbot.

File Structure
app.py: Contains the Streamlit frontend code. This file handles the user interface and displays the chatbot's responses.

backend.py: Contains all the core logic, including the RAG pipeline, API calls to Gemini, and the functions for data retrieval and content generation.

.env: A hidden file for securely storing your API key.

Technologies Used
Python: The core programming language.

Google Gemini API: For generating empathetic and context-aware responses.

Streamlit: For building the interactive web application.

DuckDuckGo Search: Used as the real-time data source for the RAG pipeline.

python-dotenv: For loading environment variables.

functools.lru_cache: For caching search results to improve performance.

License
This project is open-source and available under the MIT License.
