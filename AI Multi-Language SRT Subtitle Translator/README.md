<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>AI SRT Subtitle Translator</title>
</head>
<body>

  <h1>🚀 AI SRT Subtitle Translator</h1>

  <p>
    This Python project translates <code>.srt</code> subtitle files from English to any language
    using local LLMs (Ollama) and cloud models (Gemini), while preserving timestamps and subtitle structure.
  </p>

  <hr>

  <h2>🎯 Overview</h2>
  <p>
    The system parses subtitle files using <code>pysrt</code>, extracts each subtitle block,
    sends only the text to an LLM for translation, and reconstructs the subtitle file
    while maintaining perfect timing and formatting.
  </p>

  <hr>

  <h2>⚙️ Features</h2>
  <ul>
    <li>🌍 Translate subtitles to any language</li>
    <li>🧠 Supports Ollama (local LLMs) + Gemini API</li>
    <li>⏱ Preserves timestamps and structure</li>
    <li>📄 Works directly with .SRT files</li>
    <li>📊 Real-time progress tracking</li>
  </ul>

  <hr>

  <h2>🧠 Tech Stack</h2>
  <ul>
    <li>Python</li>
    <li>pysrt</li>
    <li>Ollama</li>
    <li>Google Gemini API</li>
    <li>OpenAI-compatible API clients</li>
  </ul>

  <hr>

  <h2>⚙️ Workflow</h2>
  <ol>
    <li>Load .SRT file using pysrt</li>
    <li>Iterate through subtitle blocks</li>
    <li>Send text to LLM (Ollama / Gemini)</li>
    <li>Receive translated text</li>
    <li>Replace original subtitle text</li>
    <li>Save new translated .SRT file</li>
  </ol>

  <hr>

  <h2>💡 Example Output</h2>

  <pre>
1
00:00:01,000 --> 00:00:03,000
Bonjour, comment ça va ?
  </pre>

  <hr>

  <h2>⚠️ Notes</h2>
  <ul>
    <li>Ensure Ollama is running locally on port 11434</li>
    <li>Set your GOOGLE_API_KEY in .env file for Gemini</li>
    <li>Translation quality depends on selected model</li>
    <li>Large files may take time to process</li>
  </ul>

  <hr>

  <h2>🚀 Future Improvements</h2>
  <ul>
    <li>Batch translation for faster performance</li>
    <li>Parallel processing for large SRT files</li>
    <li>GUI interface for non-technical users</li>
    <li>Auto language detection</li>
  </ul>

</body>
</html>
