# 🧠 AI Exam Chatbot

AI Exam Chatbot is an intelligent examination system built using Python, Gradio, SQLite, and Ollama.  
The chatbot asks random Machine Learning and Deep Learning questions, receives student answers, and evaluates them automatically using a local LLM model.

---

## ✨ Features

- Random question generation
- Interactive chatbot interface
- AI-based automatic grading
- SQLite database integration
- JSON scoring and feedback
- Local LLM inference using Ollama

---

## 🛠 Technologies Used

- Python
- Gradio
- SQLite
- Ollama
- OpenAI Python SDK
- Gemma Model

---

## ⚙️ System Workflow

1. Create SQLite database
2. Store questions and answers
3. Fetch random questions
4. Ask questions using chatbot UI
5. Collect student responses
6. Evaluate answers using AI
7. Return final score and feedback

---

## 📦 Installation

Install required libraries:

```bash
pip install openai gradio python-dotenv requests
