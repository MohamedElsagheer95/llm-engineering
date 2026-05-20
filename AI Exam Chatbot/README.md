<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AI Exam Chatbot</title>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    body{
      font-family: Arial, sans-serif;
      background:#f5f7fb;
      color:#333;
      padding:40px 20px;
    }

    .container{
      max-width:900px;
      margin:auto;
      background:#fff;
      border-radius:15px;
      padding:40px;
      box-shadow:0 5px 20px rgba(0,0,0,0.08);
    }

    h1{
      color:#2563eb;
      margin-bottom:20px;
      text-align:center;
    }

    h2{
      margin-top:30px;
      margin-bottom:15px;
      color:#1e3a8a;
    }

    p{
      margin-bottom:15px;
      line-height:1.7;
    }

    ul,ol{
      padding-left:25px;
      line-height:1.8;
    }

    code{
      background:#eef2ff;
      padding:3px 6px;
      border-radius:5px;
      color:#1e40af;
    }

    pre{
      background:#111827;
      color:#f9fafb;
      padding:15px;
      border-radius:10px;
      overflow-x:auto;
      margin-top:10px;
    }

    .footer{
      text-align:center;
      margin-top:40px;
      color:#777;
      font-size:14px;
    }
  </style>
</head>

<body>

  <div class="container">

    <h1>🧠 AI Exam Chatbot</h1>

    <p>
      AI Exam Chatbot is an intelligent examination system built using
      Python, Gradio, SQLite, and Ollama.
      The chatbot asks random AI and Machine Learning questions,
      receives student answers, and evaluates them automatically using a local LLM model.
    </p>

    <h2>✨ Features</h2>

    <ul>
      <li>Random question generation</li>
      <li>Interactive chatbot interface</li>
      <li>Automatic AI-based grading</li>
      <li>SQLite database integration</li>
      <li>JSON feedback and scoring system</li>
      <li>Runs locally using Ollama</li>
    </ul>

    <h2>🛠 Technologies</h2>

    <ul>
      <li>Python</li>
      <li>Gradio</li>
      <li>SQLite</li>
      <li>Ollama</li>
      <li>OpenAI SDK</li>
      <li>Gemma Model</li>
    </ul>

    <h2>⚙️ System Workflow</h2>

    <ol>
      <li>Create SQLite database</li>
      <li>Insert questions and answers</li>
      <li>Select random questions</li>
      <li>Ask questions using chatbot UI</li>
      <li>Collect student responses</li>
      <li>Evaluate answers using AI</li>
      <li>Display scores and feedback</li>
    </ol>

    <h2>📦 Installation</h2>

    <p>Install required libraries:</p>

    <pre>
pip install openai gradio python-dotenv requests
    </pre>

    <p>Run Ollama model locally:</p>

    <pre>
ollama run gemma4
    </pre>

    <h2>▶️ Run Application</h2>

    <pre>
python app.py
    </pre>

    <p>
      After running the application, the Gradio interface will open in your browser.
    </p>

    <h2>📊 Example Result</h2>

    <pre>
{
  "results": [
    {
      "question": "What is Deep Learning?",
      "score": 9,
      "is_correct": true,
      "feedback": "Excellent answer."
    }
  ],
  "final_score": 9
}
    </pre>

    <h2>🚀 Future Improvements</h2>

    <ul>
      <li>Voice-based exam support</li>
      <li>User authentication system</li>
      <li>Exam timer</li>
      <li>Save student history</li>
      <li>PDF export for results</li>
      <li>Advanced evaluation metrics</li>
    </ul>

    <div class="footer">
      Developed with ❤️ using Python, Gradio, SQLite, and Ollama
    </div>

  </div>

</body>
</html>
