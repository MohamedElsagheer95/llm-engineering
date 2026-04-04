

<h1>⚽ AI-Powered Football League Scraper & Formatter</h1>

<p>
A powerful Python project that combines <b>web scraping</b>, <b>LLMs</b>, and <b>data formatting</b> 
to extract football league standings from dynamic websites and present them in a clean, structured format.
</p>

<h2>🚀 Features</h2>
<ul>
<li>🌐 Scrape JavaScript-heavy websites using Selenium</li>
<li>🧠 Use LLMs (Gemini API)</li>
<li>📊 Generate structured league tables</li>
<li>🥇 Highlight top 3 teams</li>
<li>📅 Display upcoming matches</li>
<li>🧹 Clean HTML using BeautifulSoup</li>
</ul>

<h2>🧰 Tech Stack</h2>
<ul>
<li>Python</li>
<li>Selenium</li>
<li>BeautifulSoup</li>
<li>OpenAI SDK (Gemini)</li>
<li>dotenv</li>
</ul>

<h2>📦 Installation</h2>
<pre><code>pip install selenium webdriver-manager beautifulsoup4 python-dotenv openai</code></pre>

<h2>🔑 Environment Variables</h2>
<pre><code>GOOGLE_API_KEY=your_api_key_here</code></pre>

<h2>🧠 How It Works</h2>
<ol>
<li>Load API key using dotenv</li>
<li>Scrape website with Selenium</li>
<li>Clean HTML using BeautifulSoup</li>
<li>Send data to Gemini model</li>
<li>Display formatted tables</li>
</ol>

<h2>⚙️ Usage</h2>
<pre><code>summary = summarize_js_website("https://www.yallakora.com/...\")</code></pre>

<h2>🏗️ Core Components</h2>
<ul>
<li><b>ScrapeWebsite</b>: Handles scraping & parsing</li>
<li><b>summarize_js_website</b>: Runs LLM formatting</li>
</ul>

<h2>⚠️ Notes</h2>
<ul>
<li>API key must start with <code>AIz</code></li>
<li>Chrome must be installed</li>
<li>Adjust sleep time if needed</li>
</ul>

<h2>🔮 Future Improvements</h2>
<ul>
<li>Support all leagues</li>
<li>Convert to API</li>
<li>Build dashboard (Streamlit)</li>
</ul>

<h2>👨‍💻 Author</h2>
<p>
  Mohamed Elsagheer<br>
AI Engineer<br>
📧 mohamed.elsagheer@eng.sohag.edu.eg
</p>

</div>
</body>
</html>

