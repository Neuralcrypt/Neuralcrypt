<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>README</title>
  <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
  <style>
    body {
      background-color: #0d1117;
      color: #c9d1d9;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
    }
    .readme-container {
      max-width: 860px;
      margin: 40px auto;
      background-color: #161b22;
      border: 1px solid #30363d;
      border-radius: 10px;
      padding: 40px 48px;
    }
    h1 {
      font-size: 2em;
      font-weight: 700;
      border-bottom: 1px solid #30363d;
      padding-bottom: 0.3em;
      margin-bottom: 0.6em;
      color: #e6edf3;
    }
    h2 {
      font-size: 1.5em;
      font-weight: 600;
      border-bottom: 1px solid #30363d;
      padding-bottom: 0.3em;
      margin-top: 1.5em;
      margin-bottom: 0.6em;
      color: #e6edf3;
    }
    h3 {
      font-size: 1.15em;
      font-weight: 600;
      margin-top: 1.2em;
      margin-bottom: 0.4em;
      color: #e6edf3;
    }
    p {
      line-height: 1.7;
      margin-bottom: 0.9em;
      color: #c9d1d9;
    }
    a {
      color: #58a6ff;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    code {
      background-color: #21262d;
      border: 1px solid #30363d;
      border-radius: 4px;
      padding: 0.15em 0.4em;
      font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace;
      font-size: 0.88em;
      color: #e6edf3;
    }
    pre {
      background-color: #21262d;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 16px;
      overflow-x: auto;
      margin-bottom: 1em;
    }
    pre code {
      background: none;
      border: none;
      padding: 0;
      font-size: 0.9em;
      color: #c9d1d9;
    }
    ul, ol {
      padding-left: 1.6em;
      margin-bottom: 0.9em;
    }
    li {
      margin-bottom: 0.3em;
      line-height: 1.7;
    }
    .badge {
      display: inline-block;
      margin-right: 6px;
      margin-bottom: 6px;
    }
    .badge img {
      height: 22px;
      border-radius: 4px;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-bottom: 1em;
      font-size: 0.95em;
    }
    th, td {
      border: 1px solid #30363d;
      padding: 8px 14px;
      text-align: left;
    }
    th {
      background-color: #21262d;
      color: #e6edf3;
      font-weight: 600;
    }
    tr:nth-child(even) {
      background-color: #1c2128;
    }
    blockquote {
      border-left: 4px solid #3d444d;
      padding: 8px 16px;
      color: #8b949e;
      margin: 1em 0;
      background-color: #1c2128;
      border-radius: 0 6px 6px 0;
    }
    hr {
      border: none;
      border-top: 1px solid #30363d;
      margin: 2em 0;
    }
    .copy-btn {
      float: right;
      background: #21262d;
      border: 1px solid #30363d;
      color: #8b949e;
      font-size: 0.75em;
      padding: 3px 10px;
      border-radius: 5px;
      cursor: pointer;
      transition: all 0.2s;
      margin-top: -4px;
    }
    .copy-btn:hover {
      background: #30363d;
      color: #c9d1d9;
    }
    .pre-wrapper {
      position: relative;
    }
    .pre-wrapper .copy-btn {
      position: absolute;
      top: 10px;
      right: 10px;
      float: none;
      margin: 0;
    }
  </style>
</head>
<body>
  <div class="readme-container">
    <!-- Badges -->
    <div style="margin-bottom: 16px;">
      <span class="badge"><img src="https://img.shields.io/badge/version-1.0.0-blue?style=flat-square" alt="version"/></span>
      <span class="badge"><img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="license"/></span>
      <span class="badge"><img src="https://img.shields.io/badge/status-active-brightgreen?style=flat-square" alt="status"/></span>
    </div>
    <h1>📦 My Awesome Project</h1>
    <p>
      A short, clear description of what this project does and who it's for.
      This project solves <strong>X problem</strong> by doing <strong>Y</strong> in a fast and simple way.
    </p>
    <blockquote>
      💡 <strong>Tip:</strong> Replace all placeholder content with your actual project details.
    </blockquote>
    <hr/>
    <h2>📋 Table of Contents</h2>
    <ul>
      <li><a href="#features">Features</a></li>
      <li><a href="#installation">Installation</a></li>
      <li><a href="#usage">Usage</a></li>
      <li><a href="#configuration">Configuration</a></li>
      <li><a href="#api">API Reference</a></li>
      <li><a href="#contributing">Contributing</a></li>
      <li><a href="#license">License</a></li>
    </ul>
    <hr/>
    <h2 id="features">✨ Features</h2>
    <ul>
      <li>⚡ Fast and lightweight</li>
      <li>🔧 Easy to configure</li>
      <li>📦 Zero dependencies</li>
      <li>🌍 Cross-platform support</li>
      <li>🔒 Secure by default</li>
    </ul>
    <hr/>
    <h2 id="installation">🚀 Installation</h2>
    <p>Clone the repository and install dependencies:</p>
    <div class="pre-wrapper">
      <button class="copy-btn" onclick="copyCode(this)">Copy</button>
      <pre><code># Clone the repository
git clone https://github.com/username/my-awesome-project.git
# Navigate into the directory
cd my-awesome-project
# Install dependencies
npm install</code></pre>
    </div>
    <hr/>
    <h2 id="usage">▶️ Usage</h2>
    <p>Run the project with the following command:</p>
    <div class="pre-wrapper">
      <button class="copy-btn" onclick="copyCode(this)">Copy</button>
      <pre><code>npm start</code></pre>
    </div>
    <p>Or use it directly in your code:</p>
    <div class="pre-wrapper">
      <button class="copy-btn" onclick="copyCode(this)">Copy</button>
      <pre><code>import MyProject from 'my-awesome-project';
const app = new MyProject({
  option1: true,
  option2: 'value',
});
app.run();</code></pre>
    </div>
    <hr/>
    <h2 id="configuration">⚙️ Configuration</h2>
    <p>You can configure the project using a <code>.env</code> file or by passing options directly.</p>
    <div class="pre-wrapper">
      <button class="copy-btn" onclick="copyCode(this)">Copy</button>
      <pre><code># .env example
PORT=3000
DEBUG=true
API_KEY=your_api_key_here</code></pre>
    </div>
    <hr/>
    <h2 id="api">📡 API Reference</h2>
    <h3><code>GET /api/items</code></h3>
    <p>Returns a list of all items.</p>
    <table>
      <thead>
        <tr>
          <th>Parameter</th>
          <th>Type</th>
          <th>Description</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td><code>limit</code></td>
          <td><code>integer</code></td>
          <td>Max number of items to return</td>
        </tr>
        <tr>
          <td><code>offset</code></td>
          <td><code>integer</code></td>
          <td>Number of items to skip</td>
        </tr>
        <tr>
          <td><code>filter</code></td>
          <td><code>string</code></td>
          <td>Filter results by keyword</td>
        </tr>
      </tbody>
    </table>
    <hr/>
    <h2 id="contributing">🤝 Contributing</h2>
    <p>Contributions are always welcome! Please follow these steps:</p>
    <ol>
      <li>Fork the repository</li>
      <li>Create your feature branch: <code>git checkout -b feature/my-feature</code></li>
      <li>Commit your changes: <code>git commit -m 'Add my feature'</code></li>
      <li>Push to the branch: <code>git push origin feature/my-feature</code></li>
      <li>Open a Pull Request</li>
    </ol>
    <hr/>
    <h2 id="license">📄 License</h2>
    <p>
      This project is licensed under the <a href="#">MIT License</a>.
      See the <code>LICENSE</code> file for details.
    </p>
    <hr/>
    <p style="text-align:center; color:#8b949e; font-size:0.88em;">
      Made with ❤️ by <a href="#">Your Name</a> · <a href="#">GitHub</a> · <a href="#">Twitter</a>
    </p>
  </div>
  <script>
    function copyCode(btn) {
      const pre = btn.nextElementSibling;
      const text = pre.innerText;
      navigator.clipboard.writeText(text).then(() => {
        btn.textContent = "Copied!";
        btn.style.color = "#3fb950";
        setTimeout(() => {
          btn.textContent = "Copy";
          btn.style.color = "";
        }, 2000);
      });
    }
  </script>
</body>
</html>
