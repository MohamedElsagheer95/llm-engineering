<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
  
</head>

<body>

<h1>YouTube AI Summarizer</h1>

<h2>Overview</h2>
<p>
This project is an AI-powered tool that extracts transcripts from YouTube videos and converts them into structured, easy-to-read summaries using Large Language Models (Gemini, GPT, or Ollama).
</p>

<h2>Features</h2>
<ul>
    <li>Extract transcripts from YouTube videos</li>
    <li>Generate structured AI summaries</li>
    <li>Support multiple LLMs (Gemini, GPT, Ollama)</li>
    <li>Real-time streaming output</li>
    <li>Markdown formatted responses</li>
</ul>

<h2>Installation</h2>
<pre>
pip install youtube-transcript-api openai python-dotenv requests ollama
</pre>

<h2>Usage</h2>
<pre>
from your_script import summerize_video

url = "https://www.youtube.com/watch?v=VIDEO_ID"
summerize_video(url)
</pre>

<h2>How It Works</h2>
<ol>
    <li>Extract video ID from YouTube URL</li>
    <li>Fetch transcript using youtube_transcript_api</li>
    <li>Format transcript into prompt</li>
    <li>Send prompt to LLM (Gemini / GPT / Ollama)</li>
    <li>Stream structured summary output</li>
</ol>

<h2>Requirements</h2>
<ul>
    <li>Python 3.8+</li>
    <li>Internet connection</li>
    <li>Ollama (optional for local models)</li>
    <li>API key for Gemini or OpenAI (optional depending on model)</li>
</ul>

<h2>Example Output</h2>
<pre>
1. Install dependencies
2. Load transcript
3. Send to LLM
4. Generate structured summary
5. Display result
</pre>


</body>
</html>
