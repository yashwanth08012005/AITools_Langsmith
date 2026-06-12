# 🚀 LangChain + Gemini + LangSmith Starter Project

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![LangChain](https://img.shields.io/badge/LangChain-Framework-green)
![Gemini](https://img.shields.io/badge/Google-Gemini-orange)
![LangSmith](https://img.shields.io/badge/LangSmith-Tracing-purple)
![Status](https://img.shields.io/badge/Status-Learning%20Project-success)

A simple project demonstrating how to integrate **Google Gemini**, **LangChain**, and **LangSmith** for building observable AI applications.

</div>

---

## 📖 Overview

This project shows how to:

- Connect Google's Gemini model to LangChain
- Configure LangSmith tracing
- Monitor LLM interactions in real-time
- Build a foundation for AI agents and LLM applications

If you're starting your journey with **Generative AI**, **LangChain**, or **AI Agents**, this project is a great first step.

---

## 🏗️ Architecture

```text
User Prompt
     │
     ▼
LangChain
     │
     ▼
Google Gemini 2.5 Flash
     │
     ▼
Response
     │
     ▼
LangSmith Tracing & Monitoring
```

---

## ✨ Features

✅ Google Gemini Integration

✅ LangChain LLM Workflow

✅ LangSmith Observability

✅ Prompt Execution Tracking

✅ Request & Response Monitoring

✅ Beginner-Friendly Setup

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|----------|
| Python | Programming Language |
| LangChain | LLM Application Framework |
| Google Gemini | Large Language Model |
| LangSmith | Monitoring & Debugging |

---

## 📂 Project Structure

```text
langchain-gemini-langsmith/
│
├── main.py
├── requirements.txt
├── README.md
└── .env
```

---

## 📦 Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/langchain-gemini-langsmith.git

cd langchain-gemini-langsmith
```

### 2️⃣ Install Dependencies

```bash
pip install -U langchain-google-genai
pip install langsmith
pip install python-dotenv
```

Or:

```bash
pip install -r requirements.txt
```

---

## 🔑 API Keys Setup

Create a `.env` file in the root directory.

```env
GOOGLE_API_KEY=your_google_api_key

LANGSMITH_API_KEY=your_langsmith_api_key

LANGSMITH_TRACING=true

LANGSMITH_PROJECT=my-langchain-project
```

---

## 💻 Example Code

```python
import os

from langchain_google_genai import ChatGoogleGenerativeAI

os.environ["LANGSMITH_TRACING"] = "true"
os.environ["LANGSMITH_PROJECT"] = "my-langchain-project"

llm = ChatGoogleGenerativeAI(
    model="gemini-2.5-flash"
)

response = llm.invoke(
    "Explain how LangSmith tracing works in one sentence."
)

print(response.content)
```

---

## ▶️ Running the Project

```bash
python main.py
```

Expected Output:

```text
LangSmith tracing captures and visualizes every step of an LLM application's execution for debugging and monitoring.
```

---

## 📊 LangSmith Monitoring

After running the project:

1. Open your LangSmith dashboard
2. Select your project
3. View execution traces
4. Inspect prompts and responses
5. Analyze latency and performance

---

## 🎯 What You'll Learn

By completing this project, you'll understand:

- How LangChain works with Gemini
- How LLM calls are executed
- How tracing improves debugging
- How AI applications are monitored in production
- Foundations for building AI Agents

---

## 🚀 Future Improvements

- [ ] Add Conversation Memory
- [ ] Add Prompt Templates
- [ ] Build a Chatbot Interface
- [ ] Integrate Vector Database
- [ ] Implement RAG Pipeline
- [ ] Add Multi-Agent Architecture
- [ ] Deploy with Streamlit

---

## 📚 Learning Resources

### LangChain
https://python.langchain.com

### Gemini API
https://ai.google.dev

### LangSmith
https://smith.langchain.com

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome.

Feel free to fork the repository and submit a pull request.

---

## 👨‍💻 Author

**Yashwanth**

Aspiring AI Engineer | Learning LangChain, RAG, AI Agents & LLM Applications

---

## ⭐ Support

If you found this project useful:

⭐ Star the repository

🍴 Fork the project

📢 Share it with others learning AI

---

> "The best way to learn AI is by building projects."
