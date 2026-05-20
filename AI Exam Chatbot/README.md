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

## ⚙️ Project Workflow

1. Create SQLite database
2. Insert questions and answers
3. Fetch random questions
4. Ask questions through chatbot UI
5. Collect student answers
6. Evaluate answers using AI
7. Display scores and feedback

---

## 📦 Installation

Install required libraries:

```bash
pip install openai gradio python-dotenv requests
```

Run Ollama locally:

```bash
ollama run gemma4
```

---


## 📊 Example Output

```json
{
  "results": [
    {
      "question": "Why is normalization important?",
      "score": 8,
      "is_correct": true,
      "feedback": "Good understanding of normalization."
    }
  ],
  "final_score": 8
}
```

---

## 🚀 Future Improvements

- Add authentication system
- Store exam history
- Voice input support
- Add exam timer
- Export results to PDF
- Improve scoring accuracy

---

## 👨‍💻 Author

Developed using Python, Gradio, SQLite, and Ollama.
