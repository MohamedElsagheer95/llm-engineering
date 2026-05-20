<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Exam Chatbot - README</title>

    <style>
        body{
            font-family: Arial, sans-serif;
            background:#f4f4f4;
            margin:0;
            padding:40px;
            line-height:1.7;
            color:#333;
        }

        .container{
            max-width:900px;
            margin:auto;
            background:white;
            padding:40px;
            border-radius:12px;
            box-shadow:0 0 10px rgba(0,0,0,0.1);
        }

        h1,h2{
            color:#1f4e79;
        }

        code{
            background:#eee;
            padding:2px 6px;
            border-radius:4px;
        }

        pre{
            background:#272822;
            color:#f8f8f2;
            padding:15px;
            border-radius:8px;
            overflow-x:auto;
        }

        ul{
            padding-left:20px;
        }

        .footer{
            margin-top:40px;
            text-align:center;
            color:gray;
        }
    </style>
</head>

<body>

<div class="container">

    <h1>🧠 AI Exam Chatbot</h1>

    <p>
        An AI-powered exam chatbot built using Python, Gradio, SQLite, and Ollama.
        The chatbot asks Machine Learning and Deep Learning questions,
        collects student answers, and automatically evaluates them using a local LLM model.
    </p>

    <h2>🚀 Features</h2>

    <ul>
        <li>Random question generation from SQLite database</li>
        <li>Interactive chatbot interface using Gradio</li>
        <li>Automatic answer evaluation using Ollama LLM</li>
        <li>JSON-based scoring and feedback</li>
        <li>Offline local AI inference</li>
    </ul>

    <h2>🛠 Technologies Used</h2>

    <ul>
        <li>Python</li>
        <li>Gradio</li>
        <li>SQLite</li>
        <li>Ollama</li>
        <li>OpenAI Python SDK</li>
        <li>Gemma Model</li>
    </ul>

    <h2>⚙️ Project Workflow</h2>

    <ol>
        <li>Create SQLite database</li>
        <li>Insert questions and answers</li>
        <li>Fetch random questions</li>
        <li>Ask questions through chatbot UI</li>
        <li>Collect student answers</li>
        <li>Evaluate answers using AI</li>
        <li>Return scores and feedback</li>
    </ol>

    <h2>📦 Installation</h2>

    <p>Install required libraries:</p>

    <pre>
pip install openai gradio python-dotenv requests
    </pre>

    <p>Run Ollama locally:</p>

    <pre>
ollama run gemma4
    </pre>

    <h2>▶️ Run the Project</h2>

    <pre>
python app.py
    </pre>

    <p>
        The Gradio interface will open automatically in your browser.
    </p>

    <h2>📊 Example Output</h2>

    <pre>
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
    </pre>

    <h2>🔮 Future Improvements</h2>

    <ul>
        <li>Add authentication system</li>
        <li>Store exam history</li>
        <li>Support voice input</li>
        <li>Add exam timer</li>
        <li>Export results to PDF</li>
        <li>Improve scoring accuracy</li>
    </ul>

    <div class="footer">
        <p>Developed using Python, Gradio, SQLite, and Ollama 🚀</p>
    </div>

</div>

</body>
</html>
