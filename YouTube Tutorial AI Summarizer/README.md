<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>YouTube AI Summarizer - README</title>
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
            margin: 40px;
            background-color: #f9f9f9;
            color: #222;
        }
        h1, h2, h3 {
            color: #111;
        }
        code {
            background: #eee;
            padding: 2px 6px;
            border-radius: 4px;
        }
        pre {
            background: #272822;
            color: #f8f8f2;
            padding: 15px;
            border-radius: 8px;
            overflow-x: auto;
        }
        .container {
            max-width: 900px;
            margin: auto;
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        .badge {
            display: inline-block;
            padding: 5px 10px;
            background: #007BFF;
            color: white;
            border-radius: 5px;
            font-size: 12px;
        }
    </style>
</head>

<body>

<div class="container">

    <h1>🎥 YouTube AI Summarizer</h1>

    <p>
        <span class="badge">Python</span>
        <span class="badge">LLM</span>
        <span class="badge">Ollama</span>
        <span class="badge">Gemini</span>
        <span class="badge">GPT</span>
    </p>

    <h2>📌 Overview</h2>
    <p>
        The <strong>YouTube AI Summarizer</strong> is an AI-powered tool that extracts transcripts from YouTube videos
        and converts them into structured, easy-to-follow technical documentation using Large Language Models (LLMs)
        such as Gemini, GPT, or Ollama.
    </p>

    <h2>⚙️ Features</h2>
    <ul>
        <li>Extract YouTube video transcripts automatically</li>
        <li>Support for multiple LLM backends (Gemini / GPT / Ollama)</li>
        <li>Structured SOP-style summarization</li>
        <li>Streaming output for real-time updates</li>
        <li>Markdown-formatted responses</li>
    </ul>

    <h2>📦 Installation</h2>
    <pre>
pip install youtube-transcript-api openai python-dotenv requests ollama
    </pre>

    <h2>🚀 Usage</h2>
    <pre>
from your_script import summerize_video

url = "https://www.youtube.com/watch?v=VIDEO_ID"
summerize_video(url)
    </pre>

    <h2>🧠 How It Works</h2>
    <ol>
        <li>Extract video ID from YouTube URL</li>
        <li>Fetch transcript using <code>youtube_transcript_api</code></li>
        <li>Format transcript into structured prompt</li>
        <li>Send to LLM (Gemini / GPT / Ollama)</li>
        <li>Stream and display structured summary</li>
    </ol>

    <h2>🧾 System Architecture</h2>
    <ul>
        <li>YouTube Transcript API → Data Extraction</li>
        <li>Python Backend → Processing Layer</li>
        <li>LLMs → Summarization Engine</li>
        <li>Markdown Renderer → Output Formatting</li>
    </ul>

    <h2>⚠️ Requirements</h2>
    <ul>
        <li>Python 3.8+</li>
        <li>Internet connection</li>
        <li>Ollama installed (optional for local models)</li>
        <li>OpenAI or Gemini API key (optional depending on model)</li>
    </ul>

    <h2>📌 Example Output</h2>
    <pre>
1. Install dependencies
2. Load video transcript
3. Send to LLM
4. Receive structured SOP
5. Display formatted markdown output
    </pre>

    <h2>📄 License</h2>
    <p>
        This project is open-source and free to use for educational and research purposes.
    </p>

    <h2>👨‍💻 Author</h2>
    <p>
        Developed as an AI-powered learning and summarization tool for YouTube tutorials.
    </p>

</div>

</body>
</html>
