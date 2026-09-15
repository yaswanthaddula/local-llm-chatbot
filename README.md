# 🤖 Clone AI – Local LLM Chatbot

A local AI chatbot built using **Python, Streamlit, Ollama, and Qwen2.5 3B**. The application provides an interactive chat interface for communicating with a locally hosted Large Language Model (LLM).

## 🚀 Features

* 💬 Interactive AI chatbot
* 🧠 Powered by **Qwen2.5:3B**
* 🖥️ Streamlit-based web interface
* 🏠 Runs the LLM locally using Ollama
* 🔒 Does not require an external AI API for basic chatbot functionality
* ⚡ Real-time AI responses
* 🔌 Communication with Ollama through its local API

## 🛠️ Technologies Used

* **Python**
* **Streamlit**
* **Ollama**
* **Qwen2.5:3B**
* **REST API**
* **Large Language Models (LLMs)**
* **Generative AI**

## 📁 Project Structure

```text
Clone-AI/
│
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

## ⚙️ Prerequisites

Before running the project, install:

* Python 3.9 or later
* Ollama
* Qwen2.5:3B model

## 🔧 Installation

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
cd Clone-AI
```

### 2. Create a Virtual Environment

For Windows:

```powershell
python -m venv .venv
```

Activate the virtual environment:

```powershell
.venv\Scripts\activate
```

### 3. Install Dependencies

```powershell
pip install -r requirements.txt
```

If `requirements.txt` is not available, install Streamlit manually:

```powershell
pip install streamlit
```

Then create the requirements file:

```powershell
pip freeze > requirements.txt
```

## 🧠 Install Qwen2.5:3B

Download the Qwen2.5 3B model using Ollama:

```powershell
ollama pull qwen2.5:3b
```

Verify that the model has been downloaded:

```powershell
ollama list
```

You should see:

```text
qwen2.5:3b
```

## ▶️ Run the Application

Make sure the virtual environment is activated and run:

```powershell
python -m streamlit run app.py
```

The application will open in your browser at:

```text
http://localhost:8501
```

## 🔄 How the Application Works

```text
User
  ↓
Streamlit Chat Interface
  ↓
Python Application
  ↓
Ollama Local API
  ↓
Qwen2.5:3B LLM
  ↓
Generated Response
  ↓
Streamlit Interface
  ↓
User
```

The user enters a prompt through the Streamlit interface. The Python application sends the prompt to the locally running Ollama service. Ollama processes the request using the **Qwen2.5:3B** model and returns the generated response to the Streamlit application.

## 💡 Example

### User Input

```text
What is Generative AI?
```

### AI Response

```text
Generative AI is a type of artificial intelligence that can create
new content such as text, images, audio, video, and code based on
patterns learned from data.
```

## 🧪 Troubleshooting

### Model Not Found

If you receive an error such as:

```text
Most likely the model 'qwen2.5:3b' is not downloaded.
```

Run:

```powershell
ollama pull qwen2.5:3b
```

Then verify:

```powershell
ollama list
```

### Test Qwen2.5 Directly

You can test the model without Streamlit:

```powershell
ollama run qwen2.5:3b
```

Then enter:

```text
Hello
```

If Qwen responds, the model is working correctly.

### Streamlit Command Not Recognized

If this command:

```powershell
streamlit run app.py
```

gives:

```text
'streamlit' is not recognized
```

use:

```powershell
python -m streamlit run app.py
```

If Streamlit is not installed:

```powershell
python -m pip install streamlit
```

## 🔮 Future Enhancements

* Add conversation history
* Add response streaming
* Support multiple local LLMs
* Add document upload
* Implement Retrieval-Augmented Generation (RAG)
* Add vector database integration
* Add voice input and output
* Add user authentication
* Deploy the application

## 🎯 Learning Outcomes

Through this project, the following concepts were explored:

* Generative AI
* Large Language Models (LLMs)
* Local LLM deployment
* Prompt-based interaction
* Ollama API integration
* Streamlit application development
* Python API integration

## 👨‍💻 Author

**Addula Yaswanth**

B.Tech – Artificial Intelligence & Data Science

## 📌 Disclaimer

This project is developed for educational and portfolio purposes. The chatbot uses the locally hosted **Qwen2.5:3B** model through Ollama, and the quality of responses depends on the capabilities of the selected model.
