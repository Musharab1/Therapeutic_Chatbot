# 🧠 Therapeutic Chatbot  

An **empathetic GenAI-powered chatbot** designed to provide **emotional support** and help users manage stress and anxiety.  
It leverages a **Retrieval-Augmented Generation (RAG) pipeline**, combining the conversational abilities of the **Google Gemini API** with **real-time DuckDuckGo search results**, making responses both **empathetic** and **up-to-date**.  

---

## ✨ Key Features  

- 💙 **Empathetic Persona** – Acts as a supportive psychological assistant, offering kind and caring responses.  
- 🔍 **Real-Time Information** – Fetches fresh, relevant knowledge via DuckDuckGo Search.  
- 🤖 **Gemini API Integration** – Powered by **Gemini 1.5 Flash** for advanced reasoning and high-quality conversational output.  
- 🛠️ **Modular Architecture** – Backend logic separated from frontend for clean, scalable code.  
- 🎨 **Streamlit Frontend** – Simple and user-friendly web interface for smooth interaction.  

---

## ⚙️ How It Works  

1. **Retrieve** – Searches real-time data from DuckDuckGo.  
2. **Augment** – Combines retrieved data with the user’s query.  
3. **Generate** – Gemini model produces a precise, empathetic, and context-aware response.  

---

## 🚀 Getting Started  

### ✅ Prerequisites  
- Python **3.8+**  
- A **Google Gemini API key** (available from [Google AI Studio](https://ai.google.dev) or Google Cloud Console).  

---

### 🔧 Installation  

Clone the repository:  
```bash
git clone https://github.com/your-username/therapeutic-chatbot.git
cd therapeutic-chatbot
```


## Install the required Python packages:
```bash
pip install -r requirements.txt
```
(If you don't have a requirements.txt file, you can generate one after installing the necessary packages: google-generativeai, duckduckgo-search, and streamlit.)

## Configuration

- Create a file named .env in your project's root directory.

- Add your Gemini API key to this file in the following format:
```bash
GOOGLE_API_KEY="your_api_key_here"
```
- Replace "your_api_key_here" with your actual API key.

## Running the Application
Run the Streamlit application from your terminal:
```bash
streamlit run app.py
```
The application will open in your web browser, and you can begin interacting with the chatbot.

## File Structure

- app.py: The Streamlit frontend code, handling the user interface and displaying responses.

- backend.py: The core logic, including the RAG pipeline, API calls, and data retrieval.

- .env: A hidden file for securely storing your API key.

- requirements.txt: (Optional) Lists all the required Python libraries.

## Technologies Used

- Python: The core programming language.

- Google Gemini API: For generating empathetic and context-aware responses.

- Streamlit: For building the interactive web application.

- DuckDuckGo Search: Used as the real-time data source for the RAG pipeline.

- python-dotenv: For loading environment variables.

- functools.lru_cache: For caching search results to improve performance.

## License
This project is open-source.
