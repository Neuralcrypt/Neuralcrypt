<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>courageous0102 / README.md</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      background-color: #0d1117;
      color: #c9d1d9;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
      font-size: 14px;
    }
    /* TOP BAR */
    .top-bar {
      background: #161b22;
      border-bottom: 1px solid #30363d;
      padding: 10px 20px;
      font-family: "SFMono-Regular", Consolas, monospace;
      font-size: 13px;
      color: #8b949e;
    }
    .top-bar span { color: #58a6ff; }
    /* MAIN WRAPPER */
    .wrapper {
      max-width: 900px;
      margin: 0 auto;
      padding: 20px 16px 60px;
    }
    /* HERO BANNER */
    .hero {
      width: 100%;
      background: linear-gradient(135deg, #8b2fc9 0%, #4a90d9 50%, #00bcd4 100%);
      border-radius: 10px;
      padding: 60px 20px 50px;
      text-align: center;
      position: relative;
      overflow: hidden;
      margin-bottom: 30px;
    }
    .hero::before {
      content: '';
      position: absolute;
      bottom: -10px; left: -5%; right: -5%;
      height: 60px;
      background: #0d1117;
      border-radius: 50% 50% 0 0 / 30px 30px 0 0;
    }
    .hero h1 {
      font-size: 3em;
      font-weight: 800;
      color: #fff;
      text-shadow: 0 2px 10px rgba(0,0,0,0.3);
      margin-bottom: 10px;
      border: none;
    }
    .hero p {
      font-size: 1.1em;
      color: rgba(255,255,255,0.9);
      font-weight: 500;
      letter-spacing: 0.5px;
    }
    /* TYPING LINE */
    .typing-section {
      text-align: center;
      margin: 20px 0 30px;
      font-size: 1.6em;
      font-weight: 700;
      font-family: "SFMono-Regular", Consolas, monospace;
      letter-spacing: 2px;
    }
    .typing-section .t1 { color: #7c3aed; }
    .typing-section .t2 { color: #7c3aed; }
    .typing-section .t3 { color: #f97316; }
    .typing-section .sep { color: #58a6ff; margin: 0 12px; }
    /* BADGES ROW */
    .badges-row {
      display: flex;
      align-items: center;
      gap: 0;
      margin-bottom: 30px;
      flex-wrap: wrap;
      gap: 4px;
    }
    .badge-item {
      display: flex;
      align-items: center;
      border: 1px solid #444c56;
      border-radius: 4px;
      overflow: hidden;
      font-family: "SFMono-Regular", Consolas, monospace;
      font-size: 11px;
      font-weight: 600;
      letter-spacing: 0.5px;
      text-transform: uppercase;
    }
    .badge-label {
      background: #2d333b;
      color: #adbac7;
      padding: 6px 10px;
    }
    .badge-count {
      background: #7c3aed;
      color: #fff;
      padding: 6px 10px;
    }
    .badge-value {
      background: #21262d;
      color: #adbac7;
      padding: 6px 10px;
    }
    .badge-error {
      background: #21262d;
      color: #f85149;
      padding: 6px 10px;
    }
    /* SECTION */
    .section {
      margin-bottom: 30px;
    }
    .section-title {
      font-size: 1.25em;
      font-weight: 700;
      color: #e6edf3;
      border-bottom: 1px solid #30363d;
      padding-bottom: 10px;
      margin-bottom: 20px;
      display: flex;
      align-items: center;
      gap: 10px;
    }
    /* CODE BLOCK */
    .code-block {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 20px 24px;
      font-family: "SFMono-Regular", Consolas, "Liberation Mono", Menlo, monospace;
      font-size: 13px;
      line-height: 1.8;
      position: relative;
      overflow-x: auto;
    }
    .copy-icon {
      position: absolute;
      top: 12px;
      right: 12px;
      background: #21262d;
      border: 1px solid #444c56;
      border-radius: 6px;
      color: #8b949e;
      width: 32px;
      height: 32px;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      font-size: 14px;
      transition: all 0.2s;
    }
    .copy-icon:hover { background: #30363d; color: #e6edf3; }
    /* Syntax colors */
    .kw { color: #ff7b72; } /* keyword: import, from, class, def, return */
    .fn { color: #d2a8ff; } /* function names */
    .st { color: #a5d6ff; } /* strings */
    .cm { color: #8b949e; font-style: italic; } /* comments */
    .nb { color: #79c0ff; } /* self, builtins */
    .nm { color: #ffa657; } /* attribute names after self. */
    .eq { color: #c9d1d9; } /* = and regular text */
    .br { color: #e6edf3; } /* brackets */
    .nu { color: #f2cc60; } /* numbers */
    /* QUOTE */
    .quote-line {
      text-align: center;
      padding: 24px 0;
      font-size: 1.05em;
      font-style: italic;
      color: #c9d1d9;
      border-bottom: 1px solid #30363d;
      margin-bottom: 24px;
    }
    /* CONNECT SECTION */
    .connect-buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 16px;
      justify-content: center;
    }
    .conn-btn {
      display: flex;
      align-items: center;
      gap: 0;
      border-radius: 4px;
      overflow: hidden;
      text-decoration: none;
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 0.5px;
      font-family: "SFMono-Regular", Consolas, monospace;
      text-transform: uppercase;
      border: 1px solid #444;
    }
    .conn-label {
      padding: 8px 12px;
      display: flex;
      align-items: center;
      gap: 6px;
    }
    .conn-action {
      padding: 8px 12px;
      font-weight: 800;
    }
    /* PIPELINE DIAGRAM */
    .pipeline-diagram {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 30px 20px;
      position: relative;
      overflow-x: auto;
      margin-bottom: 20px;
    }
    .pipeline-nodes {
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      gap: 0;
      min-width: 700px;
    }
    .pipe-node {
      background: #21262d;
      border: 1px solid #444c56;
      border-radius: 4px;
      padding: 8px 14px;
      font-size: 12px;
      color: #c9d1d9;
      white-space: nowrap;
      font-family: "SFMono-Regular", Consolas, monospace;
    }
    .pipe-arrow {
      color: #444c56;
      font-size: 16px;
      padding: 0 4px;
    }
    .pipeline-controls {
      position: absolute;
      top: 12px;
      right: 12px;
      display: flex;
      flex-direction: column;
      gap: 4px;
    }
    .ctrl-row {
      display: flex;
      gap: 4px;
    }
    .ctrl-btn {
      background: #21262d;
      border: 1px solid #444c56;
      border-radius: 4px;
      width: 28px;
      height: 28px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #8b949e;
      cursor: pointer;
      font-size: 12px;
    }
    .ctrl-btn:hover { background: #30363d; }
    /* EXPERTISE CARDS */
    .expertise-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      border: 1px solid #30363d;
      border-radius: 8px;
      overflow: hidden;
      margin-bottom: 20px;
    }
    .exp-card {
      border-right: 1px solid #30363d;
      padding: 24px 16px;
      text-align: center;
      background: #161b22;
    }
    .exp-card:last-child { border-right: none; }
    .exp-icon { font-size: 2.5em; margin-bottom: 12px; }
    .exp-title {
      font-weight: 700;
      color: #e6edf3;
      margin-bottom: 12px;
      font-size: 0.95em;
    }
    .exp-items {
      list-style: none;
      color: #8b949e;
      font-size: 0.82em;
      line-height: 1.8;
    }
    /* TECH STACK */
    .tech-section { margin-bottom: 20px; }
    .tech-subtitle {
      font-size: 1em;
      font-weight: 700;
      color: #e6edf3;
      margin-bottom: 12px;
      display: flex;
      align-items: center;
      gap: 8px;
    }
    .tech-badges {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      justify-content: center;
      margin-bottom: 16px;
    }
    .tech-badge {
      display: flex;
      align-items: center;
      gap: 6px;
      padding: 7px 14px;
      border-radius: 4px;
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 0.5px;
      font-family: "SFMono-Regular", Consolas, monospace;
      text-transform: uppercase;
      color: #fff;
      border: none;
    }
    .tech-badge img, .tech-badge svg { width: 16px; height: 16px; }
    /* GITHUB STATS */
    .stats-container {
      display: flex;
      gap: 16px;
      flex-wrap: wrap;
      justify-content: center;
      margin-top: 16px;
    }
    .stats-card {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 20px 24px;
      min-width: 260px;
    }
    .stats-title {
      color: #58a6ff;
      font-weight: 600;
      margin-bottom: 14px;
      font-size: 0.95em;
    }
    .stat-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 5px 0;
      font-size: 0.85em;
      border-bottom: 1px solid #21262d;
    }
    .stat-row:last-child { border-bottom: none; }
    .stat-label { color: #8b949e; display: flex; align-items: center; gap: 6px; }
    .stat-val { color: #58a6ff; font-weight: 700; }
    /* STREAK CARD */
    .streak-card {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 8px;
      padding: 20px 24px;
      min-width: 260px;
      text-align: center;
    }
    .streak-num {
      font-size: 2.5em;
      font-weight: 800;
      color: #f97316;
    }
    .streak-label { color: #8b949e; font-size: 0.85em; margin-top: 4px; }
    /* CIRCULAR PROGRESS */
    .circle-progress {
      width: 80px;
      height: 80px;
      margin: 0 auto 8px;
    }
    circle { transition: stroke-dashoffset 1s ease; }
    hr.divider {
      border: none;
      border-top: 1px solid #30363d;
      margin: 28px 0;
    }
    @media (max-width: 640px) {
      .expertise-grid { grid-template-columns: repeat(2, 1fr); }
      .hero h1 { font-size: 2em; }
      .typing-section { font-size: 1.1em; }
      .pipeline-nodes { min-width: 600px; }
    }
  </style>
</head>
<body>
<!-- TOP BAR -->
<div class="top-bar">
  courageous0102 / <span>README.md</span>
</div>
<div class="wrapper">
  <!-- HERO BANNER -->
  <div class="hero">
    <h1>Abhishek Prasad</h1>
    <p>AI Engineer &nbsp;|&nbsp; ML Enthusiast &nbsp;|&nbsp; Data Scientist</p>
  </div>
  <!-- TYPING LINE -->
  <div class="typing-section">
    <span class="t1">LLMs</span>
    <span class="sep">|</span>
    <span class="t2">RAG</span>
    <span class="sep">|</span>
    <span class="t3">Deep Learning</span>
    &nbsp;🤖
  </div>
  <!-- BADGES ROW -->
  <div class="badges-row">
    <div class="badge-item">
      <span class="badge-label">NEURAL NETWORK VISITORS</span>
      <span class="badge-count">44</span>
    </div>
    <div style="width:6px;"></div>
    <div class="badge-item">
      <span class="badge-label">AI COLLABORATORS</span>
      <span class="badge-value" id="followers-val">Loading...</span>
    </div>
    <div style="width:6px;"></div>
    <div class="badge-item">
      <span class="badge-error">UNABLE TO SELECT NEXT GITHUB TOKEN FROM POOL</span>
    </div>
  </div>
  <hr class="divider"/>
  <!-- ABOUT ME -->
  <div class="section">
    <div class="section-title">🧠 About Me - Neural Network Profile</div>
    <div class="code-block">
      <div class="copy-icon" onclick="copyCode(this)" title="Copy">⧉</div>
      <div>
        <span class="kw">import</span> <span class="eq"> tensorflow </span><span class="kw">as</span><span class="eq"> tf</span>
      </div>
      <div>
        <span class="kw">import</span><span class="eq"> numpy </span><span class="kw">as</span><span class="eq"> np</span>
      </div>
      <div>
        <span class="kw">from</span><span class="eq"> datetime </span><span class="kw">import</span><span class="eq"> datetime</span>
      </div>
      <br/>
      <div><span class="kw">class</span> <span class="fn">AIEngineer</span><span class="eq">:</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">def</span> <span class="fn">__init__</span><span class="eq">(</span><span class="nb">self</span><span class="eq">):</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="cm"># Personal Metadata</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">name</span><span class="eq"> = </span><span class="st">"Abhishek Prasad"</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">username</span><span class="eq"> = </span><span class="st">"courageous0102"</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">role</span><span class="eq"> = </span><span class="st">"AI/ML Engineer & Data Scientist"</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">status</span><span class="eq"> = </span><span class="st">"B.Tech CSE - 3rd Year"</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">experience_years</span><span class="eq"> = </span><span class="nu">2</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">email</span><span class="eq"> = </span><span class="st">"abhip9835@gmail.com"</span></div>
      <br/>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="cm"># Neural Network Architecture</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">skills</span><span class="eq"> = </span><span class="br">{</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'programming'</span><span class="eq">: [</span><span class="st">'Python'</span><span class="eq">, </span><span class="st">'Java'</span><span class="eq">, </span><span class="st">'C'</span><span class="eq">, </span><span class="st">'C++'</span><span class="eq">],</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'ml_frameworks'</span><span class="eq">: [</span><span class="st">'TensorFlow'</span><span class="eq">, </span><span class="st">'PyTorch'</span><span class="eq">, </span><span class="st">'Keras'</span><span class="eq">, </span><span class="st">'Scikit-learn'</span><span class="eq">],</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'ai_domains'</span><span class="eq">: [</span><span class="st">'Deep Learning'</span><span class="eq">, </span><span class="st">'NLP'</span><span class="eq">, </span><span class="st">'Computer Vision'</span><span class="eq">, </span><span class="st">'LLMs'</span><span class="eq">],</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'data_science'</span><span class="eq">: [</span><span class="st">'Pandas'</span><span class="eq">, </span><span class="st">'NumPy'</span><span class="eq">, </span><span class="st">'Matplotlib'</span><span class="eq">, </span><span class="st">'Plotly'</span><span class="eq">],</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'cloud'</span><span class="eq">: [</span><span class="st">'AWS'</span><span class="eq">, </span><span class="st">'GCP'</span><span class="eq">],</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'specialization'</span><span class="eq">: [</span><span class="st">'RAG'</span><span class="eq">, </span><span class="st">'Transformers'</span><span class="eq">, </span><span class="st">'Model Optimization'</span><span class="eq">]</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="br">}</span></div>
      <br/>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="cm"># Current Training Loop</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">learning_pipeline</span><span class="eq"> = [</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"🎯 Advanced Machine Learning Algorithms"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"🚀 Deep Neural Networks & Architectures"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"💬 Large Language Models (LLMs)"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"🔗 Retrieval-Augmented Generation (RAG)"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"☁️ Cloud ML Deployment (AWS SageMaker)"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"🚀 MLOps & Model Production"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="eq">]</span></div>
      <br/>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="cm"># Model Performance Metrics</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="nb">self</span><span class="eq">.</span><span class="nm">achievements</span><span class="eq"> = </span><span class="br">{</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'accuracy'</span><span class="eq">: </span><span class="st">'High'</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'passion'</span><span class="eq">: </span><span class="st">'Maximum'</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'collaboration'</span><span class="eq">: </span><span class="st">'Always Open'</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">'innovation'</span><span class="eq">: </span><span class="st">'Continuous'</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="br">}</span></div>
      <br/>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">def</span> <span class="fn">forward_pass</span><span class="eq">(</span><span class="nb">self</span><span class="eq">):</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"""Processing current projects and learning"""</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="eq">projects = [</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"Building production-ready ML models"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"Implementing LLMs in real-world applications"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"Creating RAG systems for intelligent retrieval"</span><span class="eq">,</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"Developing AI-powered solutions"</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="eq">]</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">return</span><span class="eq"> projects</span></div>
      <br/>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">def</span> <span class="fn">backward_propagation</span><span class="eq">(</span><span class="nb">self</span><span class="eq">):</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"""Learning from feedback and improving"""</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">return</span> <span class="st">"Always optimizing through collaboration and feedback!"</span></div>
      <br/>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">def</span> <span class="fn">predict_future</span><span class="eq">(</span><span class="nb">self</span><span class="eq">):</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"""My vision for the future"""</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">return</span> <span class="st">"Creating AI systems that make a real impact 🚀"</span></div>
      <br/>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">def</span> <span class="fn">connect</span><span class="eq">(</span><span class="nb">self</span><span class="eq">):</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="st">"""Let's collaborate!"""</span></div>
      <div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="kw">return</span> <span class="st">f"🌐 Reach me at: {self.email}"</span></div>
      <br/>
      <div><span class="cm"># Initialize the model</span></div>
      <div><span class="eq">abhishek = </span><span class="fn">AIEngineer</span><span class="eq">()</span></div>
      <div><span class="fn">print</span><span class="eq">(abhishek.</span><span class="nm">predict_future</span><span class="eq">())</span></div>
      <div><span class="fn">print</span><span class="eq">(abhishek.</span><span class="nm">connect</span><span class="eq">())</span></div>
    </div>
  </div>
  <!-- QUOTE -->
  <div class="quote-line">
    💡 &nbsp;<em>"Turning data into intelligence, one model at a time"</em>
  </div>
  <!-- CONNECT & COLLABORATE -->
  <div class="section">
    <div class="section-title">🌐 Connect & Collaborate</div>
    <div class="connect-buttons">
      <a href="#" class="conn-btn" style="border-color:#555;">
        <span class="conn-label" style="background:#2d333b; color:#adbac7;">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="#0077b5"><path d="M20.45 20.45H16.9v-5.57c0-1.33-.03-3.04-1.85-3.04-1.85 0-2.13 1.45-2.13 2.94v5.67H9.37V8.99h3.41v1.56h.05c.48-.9 1.63-1.85 3.36-1.85 3.59 0 4.25 2.36 4.25 5.43v6.32zM5.34 7.43a2 2 0 1 1 0-4 2 2 0 0 1 0 4zm1.82 13.02H3.52V8.99h3.64v11.46zM22.23 0H1.77C.79 0 0 .77 0 1.72v20.56C0 23.23.79 24 1.77 24h20.46C23.21 24 24 23.23 24 22.28V1.72C24 .77 23.21 0 22.23 0z"/></svg>
          LINKEDIN
        </span>
        <span class="conn-action" style="background:#0077b5; color:#fff;">CONNECT</span>
      </a>
      <a href="#" class="conn-btn" style="border-color:#555;">
        <span class="conn-label" style="background:#2d333b; color:#adbac7;">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="url(#ig)"><defs><linearGradient id="ig" x1="0%" y1="100%" x2="100%" y2="0%"><stop offset="0%" style="stop-color:#f09433"/><stop offset="25%" style="stop-color:#e6683c"/><stop offset="50%" style="stop-color:#dc2743"/><stop offset="75%" style="stop-color:#cc2366"/><stop offset="100%" style="stop-color:#bc1888"/></linearGradient></defs><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zM12 0C8.741 0 8.333.014 7.053.072 2.695.272.273 2.69.073 7.052.014 8.333 0 8.741 0 12c0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98C8.333 23.986 8.741 24 12 24c3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98C15.668.014 15.259 0 12 0zm0 5.838a6.162 6.162 0 1 0 0 12.324 6.162 6.162 0 0 0 0-12.324zM12 16a4 4 0 1 1 0-8 4 4 0 0 1 0 8zm6.406-11.845a1.44 1.44 0 1 0 0 2.881 1.44 1.44 0 0 0 0-2.881z"/></svg>
          INSTAGRAM
        </span>
        <span class="conn-action" style="background:linear-gradient(45deg,#f09433,#e6683c,#dc2743,#cc2366,#bc1888); color:#fff;">FOLLOW</span>
      </a>
      <a href="mailto:abhip9835@gmail.com" class="conn-btn" style="border-color:#555;">
        <span class="conn-label" style="background:#2d333b; color:#adbac7;">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="#EA4335"><path d="M24 5.457v13.909c0 .904-.732 1.636-1.636 1.636h-3.819V11.73L12 16.64l-6.545-4.91v9.273H1.636A1.636 1.636 0 0 1 0 19.366V5.457c0-2.023 2.309-3.178 3.927-1.964L5.455 4.64 12 9.548l6.545-4.91 1.528-1.145C21.69 2.28 24 3.434 24 5.457z"/></svg>
          GMAIL
        </span>
        <span class="conn-action" style="background:#EA4335; color:#fff;">CONTACT</span>
      </a>
      <a href="#" class="conn-btn" style="border-color:#555;">
        <span class="conn-label" style="background:#2d333b; color:#adbac7;">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="#ff6600"><polygon points="12,2 15.09,8.26 22,9.27 17,14.14 18.18,21.02 12,17.77 5.82,21.02 7,14.14 2,9.27 8.91,8.26"/></svg>
          PORTFOLIO
        </span>
        <span class="conn-action" style="background:#ff6600; color:#fff;">VISIT</span>
      </a>
    </div>
  </div>
  <hr class="divider"/>
  <!-- CURRENT LEARNING PIPELINE -->
  <div class="section">
    <div class="section-title">🎯 Current Learning Pipeline</div>
    <div class="pipeline-diagram">
      <div class="pipeline-controls">
        <div class="ctrl-row">
          <div class="ctrl-btn">↔</div>
          <div class="ctrl-btn">⧉</div>
        </div>
        <div class="ctrl-row">
          <div class="ctrl-btn" style="grid-column:1;">↑</div>
          <div class="ctrl-btn">⊕</div>
        </div>
        <div class="ctrl-row">
          <div class="ctrl-btn">←</div>
          <div class="ctrl-btn">↺</div>
          <div class="ctrl-btn">→</div>
        </div>
        <div class="ctrl-row">
          <div class="ctrl-btn">↓</div>
          <div class="ctrl-btn">⊖</div>
        </div>
      </div>
      <div style="overflow-x:auto;">
        <div style="display:flex; flex-direction:column; align-items:flex-start; min-width:700px;">
          <!-- top row: Evaluation, Deployment, Monitoring -->
          <div style="display:flex; align-items:center; margin-left:430px; margin-bottom:4px;">
            <div class="pipe-node">Evaluation</div>
            <div class="pipe-arrow">→</div>
            <div class="pipe-node">Deployment</div>
            <div class="pipe-arrow">→</div>
            <div class="pipe-node">Monitoring</div>
          </div>
          <!-- main row -->
          <div style="display:flex; align-items:center; gap:0;">
            <div class="pipe-node">Data</div>
            <div class="pipe-arrow">→</div>
            <div class="pipe-node">Preprocessing</div>
            <div class="pipe-arrow">→</div>
            <div class="pipe-node">Feature Engineering</div>
            <div class="pipe-arrow">→</div>
            <div class="pipe-node">Model Training</div>
            <div class="pipe-arrow" style="margin-right:4px;">↗</div>
            <div style="width:220px;"></div>
            <div class="pipe-node">Optimization</div>
          </div>
          <!-- loop back arrow hint -->
          <div style="margin-left:430px; font-size:11px; color:#444c56; margin-top:2px;">↙ feedback loop</div>
        </div>
      </div>
    </div>
    <!-- EXPERTISE GRID -->
    <div class="expertise-grid">
      <div class="exp-card">
        <div class="exp-icon">🧠</div>
        <div class="exp-title">Machine<br/>Learning</div>
        <ul class="exp-items">
          <li>Supervised &</li>
          <li>Unsupervised Learning</li>
          <li>Model Optimization</li>
          <li>Feature Engineering</li>
        </ul>
      </div>
      <div class="exp-card">
        <div class="exp-icon">🕸️</div>
        <div class="exp-title">Deep Learning</div>
        <ul class="exp-items">
          <li>Neural Networks</li>
          <li>CNNs & RNNs</li>
          <li>Transfer Learning</li>
        </ul>
      </div>
      <div class="exp-card">
        <div class="exp-icon">🤖</div>
        <div class="exp-title">LLMs & NLP</div>
        <ul class="exp-items">
          <li>GPT Models</li>
          <li>RAG Systems</li>
          <li>Fine-tuning</li>
        </ul>
      </div>
      <div class="exp-card">
        <div class="exp-icon">☁️</div>
        <div class="exp-title">Cloud & MLOps</div>
        <ul class="exp-items">
          <li>AWS SageMaker</li>
          <li>Model Deployment</li>
          <li>CI/CD Pipelines</li>
        </ul>
      </div>
    </div>
  </div>
  <hr class="divider"/>
  <!-- TECH STACK -->
  <div class="section">
    <div class="section-title">💻 Tech Stack - AI/ML Arsenal</div>
    <div class="tech-section">
      <div class="tech-subtitle">🤖 AI/ML & Data Science</div>
      <div class="tech-badges">
        <span class="tech-badge" style="background:#3776ab;">🐍 PYTHON</span>
        <span class="tech-badge" style="background:#ff6f00;">🔺 TENSORFLOW</span>
        <span class="tech-badge" style="background:#ee4c2c;">🔥 PYTORCH</span>
        <span class="tech-badge" style="background:#d00000;">K KERAS</span>
        <span class="tech-badge" style="background:#f7931e; color:#000;">⚙️ SCIKIT-LEARN</span>
        <span class="tech-badge" style="background:#6b4e9e;">🐼 PANDAS</span>
        <span class="tech-badge" style="background:#4dabcf; color:#000;">🔢 NUMPY</span>
        <span class="tech-badge" style="background:#11557c;">📊 MATPLOTLIB</span>
        <span class="tech-badge" style="background:#3f4f75;">📈 PLOTLY</span>
        <span class="tech-badge" style="background:#5c3ee8;">👁️ OPENCV</span>
        <span class="tech-badge" style="background:#ffd21e; color:#000;">🤗 HUGGING FACE</span>
      </div>
    </div>
    <div class="tech-section">
      <div class="tech-subtitle">👨‍💻 Programming Languages</div>
      <div class="tech-badges">
        <span class="tech-badge" style="background:#3776ab;">🐍 PYTHON</span>
        <span class="tech-badge" style="background:#f89820;">☕ JAVA</span>
        <span class="tech-badge" style="background:#555;">C C</span>
        <span class="tech-badge" style="background:#00599c;">C C++</span>
        <span class="tech-badge" style="background:#e34c26;">🖥️ HTML5</span>
        <span class="tech-badge" style="background:#1572b6; color:#fff;">CSS3</span>
        <span class="tech-badge" style="background:#f0db4f; color:#000;">JS JAVASCRIPT</span>
      </div>
    </div>
    <div class="tech-section">
      <div class="tech-subtitle">☁️ Cloud & Deployment</div>
      <div class="tech-badges">
        <span class="tech-badge" style="background:#ff9900; color:#000;">AWS</span>
        <span class="tech-badge" style="background:#4285f4;">☁️ GOOGLE CLOUD</span>
        <span class="tech-badge" style="background:#ff4b4b;">🎈 STREAMLIT</span>
        <span class="tech-badge" style="background:#1a1a1a; border:1px solid #555;">🌶️ FLASK</span>
        <span class="tech-badge" style="background:#009688;">⚡ FASTAPI</span>
        <span class="tech-badge" style="background:#2496ed;">🐳 DOCKER</span>
      </div>
    </div>
    <div class="tech-section">
      <div class="tech-subtitle">🛠️ Tools & Platforms</div>
      <div class="tech-badges">
        <span class="tech-badge" style="background:#f37626;">📓 JUPYTER</span>
        <span class="tech-badge" style="background:#f9ab00; color:#000;">∞ GOOGLE COLAB</span>
        <span class="tech-badge" style="background:#007acc;">VS CODE</span>
        <span class="tech-badge" style="background:#f05032;">⎇ GIT</span>
        <span class="tech-badge" style="background:#1a1a1a; border:1px solid #555;">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="#fff"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z"/></svg>
          GITHUB
        </span>
        <span class="tech-badge" style="background:#44a833;">🐍 ANACONDA</span>
      </div>
    </div>
    <div class="tech-section">
      <div class="tech-subtitle">🗄️ Databases</div>
      <div class="tech-badges">
        <span class="tech-badge" style="background:#47a248;">🍃 MONGODB</span>
        <span class="tech-badge" style="background:#4479a1;">🐬 MYSQL</span>
        <span class="tech-badge" style="background:#336791;">🐘 POSTGRESQL</span>
        <span class="tech-badge" style="background:#cc2927;">MICROSOFT SQL SERVER</span>
      </div>
    </div>
  </div>
  <hr class="divider"/>
  <!-- GITHUB ANALYTICS -->
  <div class="section">
    <div class="section-title">📊 GitHub Analytics - Model Performance Metrics</div>
    <div class="stats-container">
      <!-- STATS CARD -->
      <div class="stats-card">
        <div class="stats-title">Abhishek prasad's GitHub Stats</div>
        <div class="stat-row">
          <span class="stat-label">⭐ Total Stars Earned:</span>
          <span class="stat-val">7</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">🕐 Total Commits:</span>
          <span class="stat-val">5</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">🔀 Total PRs:</span>
          <span class="stat-val">0</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">⚠️ Total Issues:</span>
          <span class="stat-val">1</span>
        </div>
        <div class="stat-row">
          <span class="stat-label">📁 Contributed to (last year):</span>
          <span class="stat-val">1</span>
        </div>
        <div style="margin-top:16px; text-align:center;">
          <svg viewBox="0 0 100 100" width="70" height="70">
            <circle cx="50" cy="50" r="40" fill="none" stroke="#21262d" stroke-width="10"/>
            <circle cx="50" cy="50" r="40" fill="none" stroke="#58a6ff" stroke-width="10"
              stroke-dasharray="251" stroke-dashoffset="220" stroke-linecap="round"
              transform="rotate(-90 50 50)"/>
            <text x="50" y="55" text-anchor="middle" fill="#58a6ff" font-size="12" font-weight="bold">C+</text>
          </svg>
        </div>
      </div>
      <!-- STREAK CARD -->
      <div class="streak-card">
        <div class="stats-title" style="text-align:left;">🔥 GitHub Streak</div>
        <div style="margin-top:20px;">
          <div class="streak-num">0</div>
          <div class="streak-label">Current Streak</div>
          <div style="margin: 20px 0; border-top: 1px solid #30363d; border-bottom: 1px solid #30363d; padding: 12px 0;">
            <div style="color:#8b949e; font-size:0.8em; margin-bottom:4px;">Total Contributions</div>
            <div style="font-size:1.5em; font-weight:700; color:#58a6ff;">6</div>
          </div>
          <div>
            <div style="color:#8b949e; font-size:0.8em; margin-bottom:4px;">Longest Streak</div>
            <div style="font-size:1.5em; font-weight:700; color:#f97316;">1 day</div>
          </div>
        </div>
      </div>
      <!-- LANGUAGE CARD -->
      <div class="stats-card">
        <div class="stats-title">Top Languages</div>
        <div style="margin-top:10px;">
          <div style="display:flex; justify-content:space-between; margin-bottom:6px;">
            <span style="color:#c9d1d9; font-size:0.85em;">Python</span>
            <span style="color:#8b949e; font-size:0.85em;">65%</span>
          </div>
          <div style="background:#21262d; border-radius:4px; height:8px; margin-bottom:12px;">
            <div style="background:#3776ab; width:65%; height:100%; border-radius:4px;"></div>
          </div>
          <div style="display:flex; justify-content:space-between; margin-bottom:6px;">
            <span style="color:#c9d1d9; font-size:0.85em;">Jupyter Notebook</span>
            <span style="color:#8b949e; font-size:0.85em;">25%</span>
          </div>
          <div style="background:#21262d; border-radius:4px; height:8px; margin-bottom:12px;">
            <div style="background:#f37626; width:25%; height:100%; border-radius:4px;"></div>
          </div>
          <div style="display:flex; justify-content:space-between; margin-bottom:6px;">
            <span style="color:#c9d1d9; font-size:0.85em;">JavaScript</span>
            <span style="color:#8b949e; font-size:0.85em;">7%</span>
          </div>
          <div style="background:#21262d; border-radius:4px; height:8px; margin-bottom:12px;">
            <div style="background:#f0db4f; width:7%; height:100%; border-radius:4px;"></div>
          </div>
          <div style="display:flex; justify-content:space-between; margin-bottom:6px;">
            <span style="color:#c9d1d9; font-size:0.85em;">Other</span>
            <span style="color:#8b949e; font-size:0.85em;">3%</span>
          </div>
          <div style="background:#21262d; border-radius:4px; height:8px;">
            <div style="background:#8b949e; width:3%; height:100%; border-radius:4px;"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <hr class="divider"/>
  <!-- FOOTER -->
  <div style="text-align:center; color:#8b949e; font-size:0.82em; margin-top:20px;">
    <p>⭐ From <a href="#" style="color:#58a6ff; text-decoration:none;">courageous0102</a> — Made with ❤️ and lots of ☕</p>
    <p style="margin-top:6px; font-family:monospace;">Last updated: <span id="last-updated"></span></p>
  </div>
</div>
<script>
  // Set last updated
  const d = new Date();
  document.getElementById('last-updated').textContent = d.toLocaleDateString('en-US', {
    year:'numeric', month:'long', day:'numeric'
  });
  // Copy code button
  function copyCode(btn) {
    const block = btn.closest('.code-block');
    let text = block.innerText.replace('⧉','').trim();
    navigator.clipboard.writeText(text).then(() => {
      btn.textContent = '✓';
      btn.style.color = '#3fb950';
      setTimeout(() => {
        btn.textContent = '⧉';
        btn.style.color = '';
      }, 2000);
    });
  }
  // Visitor counter animation
  let count = 0;
  const target = 44;
  const interval = setInterval(() => {
    count += 2;
    if (count >= target) { count = target; clearInterval(interval); }
    document.querySelectorAll('.badge-count').forEach(el => el.textContent = count);
  }, 30);
  // Simulate followers count
  document.getElementById('followers-val').textContent = '3';
</script>
</body>
</html>
