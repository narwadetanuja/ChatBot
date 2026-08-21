# 🤖 Tanuu Chatbot

A simple AI-powered chatbot built using **Python, Streamlit, and Google Gemini API**.
The chatbot allows users to interact with an AI assistant through a clean and simple web interface.

## 🚀 Features

* 💬 Interactive AI chatbot
* 🤖 Powered by Google Gemini
* 🖥️ Simple Streamlit interface
* 📱 User-friendly design
* ⚡ Fast responses
* 🧠 Maintains chat history during the session

## 🛠️ Technologies Used

* Python
* Streamlit
* Google Gemini API
* Google GenAI SDK

## 📂 Project Structure

```text
Tanuu-Chatbot/
│
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

### 3. Activate the virtual environment

**Windows:**

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Add your API key securely

Do **not** put your API key directly in `app.py`.

For Streamlit deployment, use:

```text
.streamlit/secrets.toml
```

Example:

```toml
GEMINI_API_KEY = "your-api-key"
```

Then access it in Python using:

```python
import streamlit as st

api_key = st.secrets["GEMINI_API_KEY"]
```

## ▶️ Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

## 🌐 Deployment

This project can be deployed using **Streamlit Community Cloud**.

1. Push the project to GitHub.
2. Connect your GitHub repository to Streamlit.
3. Select `app.py` as the main file.
4. Add your Gemini API key in Streamlit Secrets.
5. Deploy the application.

## 🔐 Security

Never upload your API key, passwords, or other secret credentials to GitHub.

Add sensitive files to `.gitignore`:

```text
.env
.streamlit/secrets.toml
venv/
__pycache__/
```
