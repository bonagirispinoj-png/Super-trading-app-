<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TradeGod — AI Options Super Analyzer</title>
<link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@400;500;600;700&family=Share+Tech+Mono&family=Orbitron:wght@400;700;900&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #030812;
    --bg2: #060f1e;
    --bg3: #0a1628;
    --accent: #00f5ff;
    --accent2: #ff3e6c;
    --accent3: #ffb800;
    --green: #00ff88;
    --red: #ff3e6c;
    --gold: #ffb800;
    --text: #c8d8f0;
    --dim: #4a6080;
    --border: rgba(0,245,255,0.15);
    --glow: 0 0 20px rgba(0,245,255,0.3);
    --glow-red: 0 0 20px rgba(255,62,108,0.3);
    --glow-gold: 0 0 20px rgba(255,184,0,0.3);
  }
  * { margin:0; padding:0; box-sizing:border-box; }
  body {
    background: var(--bg);
    color: var(--text);
    font-family: 'Rajdhani', sans-serif;
    min-height: 100vh;
    overflow-x: hidden;
  }
  body::before {
    content:'';
    position:fixed;
    inset:0;
    background: 
      radial-gradient(ellipse 80% 40% at 50% -10%, rgba(0,245,255,0.07) 0%, transparent 60%),
      radial-gradient(ellipse 60% 30% at 100% 80%, rgba(255,62,108,0.05) 0%, transparent 50%),
      repeating-linear-gradient(0deg, transparent, transparent 39px, rgba(0,245,255,0.03) 40px),
      repeating-linear-gradient(90deg, transparent, transparent 39px, rgba(0,245,255,0.03) 40px);
    pointer-events:none;
    z-index:0;
  }

  /* HEADER */
  .header {
    position:relative;
    z-index:10;
    text-align:center;
    padding: 24px 16px 16px;
    border-bottom: 1px solid var(--border);
    background: linear-gradient(180deg, rgba(0,245,255,0.05) 0%, transparent 100%);
  }
  .logo {
    font-family:'Orbitron',sans-serif;
    font-size:28px;
    font-weight:900;
    letter-spacing:4px;
    background: linear-gradient(135deg, var(--accent) 0%, var(--accent2) 100%);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
    text-shadow: none;
    filter: drop-shadow(0 0 15px rgba(0,245,255,0.5));
  }
  .tagline {
    font-size:11px;
    letter-spacing:3px;
    color:var(--dim);
    margin-top:4px;
    font-family:'Share Tech Mono',monospace;
  }
  .live-badge {
    display:inline-flex;
    align-items:center;
    gap:6px;
    background:rgba(0,255,136,0.1);
    border:1px solid rgba(0,255,136,0.3);
    border-radius:20px;
    padding:3px 10px;
    font-size:10px;
    color:var(--green);
    font-family:'Share Tech Mono',monospace;
    margin-top:8px;
    letter-spacing:2px;
  }
  .live-dot {
    width:6px;height:6px;
    border-radius:50%;
    background:var(--green);
    animation:pulse 1.2s ease-in-out infinite;
  }
  @keyframes pulse { 0%,100%{opacity:1;transform:scale(1)} 50%{opacity:0.4;transform:scale(0.8)} }

  /* TABS */
  .tabs {
    display:flex;
    overflow-x:auto;
    gap:4px;
    padding:12px 12px 0;
    position:relative;
    z-index:10;
    scrollbar-width:none;
  }
  .tabs::-webkit-scrollbar{display:none;}
  .tab {
    flex-shrink:0;
    padding:8px 14px;
    border-radius:8px 8px 0 0;
    border:1px solid var(--border);
    border-bottom:none;
    background:var(--bg2);
    color:var(--dim);
    font-size:11px;
    font-weight:600;
    letter-spacing:1px;
    cursor:pointer;
    transition:all 0.2s;
    font-family:'Rajdhani',sans-serif;
    white-space:nowrap;
  }
  .tab.active {
    background:var(--bg3);
    color:var(--accent);
    border-color:rgba(0,245,255,0.3);
    box-shadow: var(--glow);
  }

  /* PANELS */
  .panel {
    display:none;
    position:relative;
    z-index:10;
    padding:16px 12px;
    animation:fadeIn 0.3s ease;
  }
  .panel.active { display:block; }
  @keyframes fadeIn { from{opacity:0;transform:translateY(4px)} to{opacity:1;transform:translateY(0)} }

  /* CARDS */
  .card {
    background:var(--bg2);
    border:1px solid var(--border);
    border-radius:12px;
    padding:16px;
    margin-bottom:12px;
    position:relative;
    overflow:hidden;
  }
  .card::before {
    content:'';
    position:absolute;
    top:0;left:0;right:0;
    height:2px;
    background:linear-gradient(90deg, var(--accent), transparent);
  }
  .card.red::before { background:linear-gradient(90deg, var(--red), transparent); }
  .card.gold::before { background:linear-gradient(90deg, var(--gold), transparent); }
  .card.green::before { background:linear-gradient(90deg, var(--green), transparent); }

  .card-title {
    font-family:'Orbitron',sans-serif;
    font-size:10px;
    letter-spacing:2px;
    color:var(--accent);
    margin-bottom:12px;
    display:flex;
    align-items:center;
    gap:8px;
  }
  .card.red .card-title { color:var(--red); }
  .card.gold .card-title { color:var(--gold); }
  .card.green .card-title { color:var(--green); }

  /* INPUTS */
  .input-grid {
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:8px;
    margin-bottom:12px;
  }
  .input-group {
    display:flex;
    flex-direction:column;
    gap:4px;
  }
  .input-group label {
    font-size:10px;
    letter-spacing:2px;
    color:var(--dim);
    font-family:'Share Tech Mono',monospace;
  }
  .inp {
    background:var(--bg3);
    border:1px solid var(--border);
    border-radius:6px;
    padding:10px 12px;
    color:var(--accent);
    font-family:'Share Tech Mono',monospace;
    font-size:14px;
    width:100%;
    outline:none;
    transition:all 0.2s;
  }
  .inp:focus {
    border-color:var(--accent);
    box-shadow:var(--glow);
  }
  select.inp option { background:var(--bg2); color:var(--text); }

  /* BUTTONS */
  .btn {
    width:100%;
    padding:14px;
    border:none;
    border-radius:8px;
    font-family:'Orbitron',sans-serif;
    font-size:12px;
    font-weight:700;
    letter-spacing:2px;
    cursor:pointer;
    transition:all 0.3s;
    position:relative;
    overflow:hidden;
  }
  .btn-primary {
    background:linear-gradient(135deg, #0066aa, #00aaff);
    color:#fff;
    box-shadow:0 4px 20px rgba(0,170,255,0.3);
  }
  .btn-primary:hover { transform:translateY(-2px); box-shadow:0 6px 30px rgba(0,170,255,0.5); }
  .btn-primary:active { transform:translateY(0); }
  .btn-danger {
    background:linear-gradient(135deg, #aa0033, #ff3e6c);
    color:#fff;
    box-shadow:0 4px 20px rgba(255,62,108,0.3);
  }
  .btn-gold {
    background:linear-gradient(135deg, #aa6600, #ffb800);
    color:#000;
    box-shadow:0 4px 20px rgba(255,184,0,0.3);
  }
  .btn-sm {
    padding:8px 16px;
    width:auto;
    font-size:10px;
  }

  /* RESULTS SECTION */
  .result-section { margin-bottom:16px; }
  .result-title {
    font-family:'Share Tech Mono',monospace;
    font-size:10px;
    letter-spacing:2px;
    color:var(--dim);
    margin-bottom:8px;
    padding-bottom:4px;
    border-bottom:1px solid var(--border);
  }

  /* LEVEL BARS */
  .level-row {
    display:flex;
    align-items:center;
    gap:10px;
    padding:6px 8px;
    border-radius:6px;
    margin-bottom:4px;
    transition:all 0.2s;
  }
  .level-row:hover { background:rgba(255,255,255,0.03); }
  .level-label {
    font-family:'Share Tech Mono',monospace;
    font-size:11px;
    width:40px;
    flex-shrink:0;
  }
  .level-bar-wrap {
    flex:1;
    height:4px;
    background:var(--bg3);
    border-radius:2px;
    overflow:hidden;
  }
  .level-bar { height:100%; border-radius:2px; transition:width 1s ease; }
  .level-price {
    font-family:'Share Tech Mono',monospace;
    font-size:12px;
    font-weight:700;
    width:60px;
    text-align:right;
    flex-shrink:0;
  }
  .level-action {
    font-size:9px;
    letter-spacing:1px;
    padding:2px 6px;
    border-radius:4px;
    flex-shrink:0;
    width:70px;
    text-align:center;
  }

  /* BIG SIGNAL */
  .signal-box {
    background:var(--bg3);
    border-radius:12px;
    padding:20px;
    text-align:center;
    border:1px solid var(--border);
    margin-bottom:12px;
    position:relative;
    overflow:hidden;
  }
  .signal-box::after {
    content:'';
    position:absolute;
    inset:0;
    background:radial-gradient(circle at 50% 50%, rgba(0,245,255,0.05) 0%, transparent 70%);
    pointer-events:none;
  }
  .signal-main {
    font-family:'Orbitron',sans-serif;
    font-size:32px;
    font-weight:900;
    letter-spacing:4px;
    margin-bottom:4px;
  }
  .signal-sub {
    font-size:12px;
    letter-spacing:2px;
    color:var(--dim);
    font-family:'Share Tech Mono',monospace;
  }

  /* STAT BARS */
  .stat-row {
    display:flex;
    align-items:center;
    gap:10px;
    margin-bottom:8px;
  }
  .stat-label { font-size:11px; width:30px; font-family:'Share Tech Mono',monospace; }
  .stat-track {
    flex:1;
    height:8px;
    background:var(--bg3);
    border-radius:4px;
    overflow:hidden;
  }
  .stat-fill {
    height:100%;
    border-radius:4px;
    transition:width 1.5s cubic-bezier(.17,.67,.38,1.2);
  }
  .stat-pct {
    font-family:'Share Tech Mono',monospace;
    font-size:12px;
    font-weight:700;
    width:40px;
    text-align:right;
  }

  /* TRADE PLAN TABLE */
  .plan-table { width:100%; border-collapse:collapse; }
  .plan-table th {
    font-family:'Share Tech Mono',monospace;
    font-size:9px;
    letter-spacing:2px;
    color:var(--dim);
    padding:6px 8px;
    text-align:left;
    border-bottom:1px solid var(--border);
  }
  .plan-table td {
    padding:8px 8px;
    font-family:'Share Tech Mono',monospace;
    font-size:12px;
    border-bottom:1px solid rgba(255,255,255,0.04);
  }
  .plan-table tr:hover td { background:rgba(255,255,255,0.02); }

  /* UPLOAD */
  .upload-zone {
    border:2px dashed rgba(0,245,255,0.2);
    border-radius:12px;
    padding:30px 20px;
    text-align:center;
    cursor:pointer;
    transition:all 0.3s;
    background:rgba(0,245,255,0.02);
  }
  .upload-zone:hover, .upload-zone.drag {
    border-color:var(--accent);
    background:rgba(0,245,255,0.06);
    box-shadow:var(--glow);
  }
  .upload-icon { font-size:36px; margin-bottom:8px; }
  .upload-text { font-size:13px; color:var(--dim); letter-spacing:1px; }
  #chartPreview {
    max-width:100%;
    border-radius:8px;
    margin-top:12px;
    display:none;
    border:1px solid var(--border);
  }

  /* TICKER */
  .ticker-row {
    display:flex;
    gap:6px;
    flex-wrap:wrap;
    margin-bottom:12px;
  }
  .ticker-chip {
    padding:4px 10px;
    border-radius:20px;
    border:1px solid var(--border);
    font-family:'Share Tech Mono',monospace;
    font-size:10px;
    cursor:pointer;
    transition:all 0.2s;
    background:var(--bg2);
    color:var(--dim);
  }
  .ticker-chip.active, .ticker-chip:hover {
    border-color:var(--accent);
    color:var(--accent);
    background:rgba(0,245,255,0.08);
  }

  /* LOADING */
  .loading {
    display:none;
    text-align:center;
    padding:30px;
  }
  .loading.show { display:block; }
  .spinner {
    width:40px;height:40px;
    border:3px solid var(--bg3);
    border-top-color:var(--accent);
    border-radius:50%;
    animation:spin 0.8s linear infinite;
    margin:0 auto 12px;
  }
  @keyframes spin{to{transform:rotate(360deg)}}
  .loading-text {
    font-family:'Share Tech Mono',monospace;
    font-size:11px;
    letter-spacing:2px;
    color:var(--dim);
    animation:blink 1.2s ease infinite;
  }
  @keyframes blink{0%,100%{opacity:1}50%{opacity:0.3}}

  /* OUTPUT */
  #ohlcOutput, #chartOutput { display:none; }
  #ohlcOutput.show, #chartOutput.show { display:block; }

  /* SCENARIO CARDS */
  .scenario {
    background:var(--bg3);
    border-radius:8px;
    padding:12px;
    margin-bottom:8px;
    border-left:3px solid var(--accent);
  }
  .scenario.bear { border-left-color:var(--red); }
  .scenario.bull { border-left-color:var(--green); }
  .scenario.neutral { border-left-color:var(--gold); }
  .scenario-title {
    font-family:'Orbitron',sans-serif;
    font-size:10px;
    letter-spacing:2px;
    margin-bottom:8px;
  }
  .scenario-grid {
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:6px;
  }
  .sg-item { }
  .sg-label { font-size:9px; color:var(--dim); letter-spacing:1px; font-family:'Share Tech Mono',monospace; }
  .sg-value { font-size:13px; font-weight:700; font-family:'Share Tech Mono',monospace; }

  /* INDICATOR GAUGE */
  .gauge-row {
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:8px 0;
    border-bottom:1px solid rgba(255,255,255,0.04);
  }
  .gauge-name { font-size:12px; font-weight:600; }
  .gauge-signal {
    font-size:10px;
    font-family:'Share Tech Mono',monospace;
    padding:3px 8px;
    border-radius:4px;
    letter-spacing:1px;
  }
  .sig-bull { background:rgba(0,255,136,0.15); color:var(--green); }
  .sig-bear { background:rgba(255,62,108,0.15); color:var(--red); }
  .sig-neutral { background:rgba(255,184,0,0.15); color:var(--gold); }

  /* ZERODHA SECTION */
  .zerodha-info {
    background:linear-gradient(135deg, rgba(0,100,180,0.1), rgba(0,245,255,0.05));
    border:1px solid rgba(0,150,255,0.2);
    border-radius:12px;
    padding:16px;
    margin-bottom:12px;
  }
  .step-item {
    display:flex;
    gap:12px;
    padding:10px 0;
    border-bottom:1px solid var(--border);
    align-items:flex-start;
  }
  .step-num {
    font-family:'Orbitron',sans-serif;
    font-size:18px;
    font-weight:900;
    color:var(--accent);
    flex-shrink:0;
    width:28px;
  }
  .step-text { font-size:12px; line-height:1.6; }
  .step-code {
    font-family:'Share Tech Mono',monospace;
    background:var(--bg3);
    padding:2px 6px;
    border-radius:4px;
    color:var(--accent);
    font-size:11px;
  }

  /* AI ANALYSIS OUTPUT */
  .ai-output {
    background:var(--bg3);
    border-radius:8px;
    padding:14px;
    font-family:'Share Tech Mono',monospace;
    font-size:11px;
    line-height:1.8;
    color:var(--text);
    white-space:pre-wrap;
    border:1px solid var(--border);
    max-height:400px;
    overflow-y:auto;
  }
  .ai-output::-webkit-scrollbar { width:4px; }
  .ai-output::-webkit-scrollbar-track { background:var(--bg2); }
  .ai-output::-webkit-scrollbar-thumb { background:var(--accent); border-radius:2px; }

  /* DISCLAIMER */
  .disclaimer {
    background:rgba(255,184,0,0.05);
    border:1px solid rgba(255,184,0,0.2);
    border-radius:8px;
    padding:10px 12px;
    font-size:10px;
    color:var(--gold);
    font-family:'Share Tech Mono',monospace;
    letter-spacing:0.5px;
    line-height:1.6;
    margin-top:12px;
  }

  /* PSYCH METER */
  .psych-gauge {
    background:var(--bg3);
    border-radius:12px;
    padding:16px;
    text-align:center;
    margin-bottom:8px;
  }
  .psych-arc {
    position:relative;
    width:160px;
    height:80px;
    margin:0 auto 12px;
    overflow:hidden;
  }
  .psych-arc svg { width:160px;height:160px; position:absolute; top:0;left:0; }

  /* SCROLLBAR */
  ::-webkit-scrollbar{width:4px;height:4px;}
  ::-webkit-scrollbar-track{background:var(--bg2);}
  ::-webkit-scrollbar-thumb{background:var(--accent);border-radius:2px;}

  .text-green{color:var(--green);}
  .text-red{color:var(--red);}
  .text-gold{color:var(--gold);}
  .text-accent{color:var(--accent);}
  .text-dim{color:var(--dim);}
  .fw7{font-weight:700;}
  .mono{font-family:'Share Tech Mono',monospace;}
  .mt8{margin-top:8px;}
  .mb8{margin-bottom:8px;}
  .flex{display:flex;}
  .flex-between{display:flex;justify-content:space-between;align-items:center;}
</style>
</head>
<body>

<div class="header">
  <div class="logo">TRADEGOD ⚡</div>
  <div class="tagline">AI-POWERED OPTIONS SUPER ANALYZER</div>
  <div class="live-badge"><span class="live-dot"></span>POWERED BY CLAUDE AI</div>
</div>

<div class="tabs">
  <div class="tab active" onclick="switchTab('ohlc')">📊 OHLC ANALYZER</div>
  <div class="tab" onclick="switchTab('chart')">📸 CHART SCANNER</div>
  <div class="tab" onclick="switchTab('zerodha')">🔗 ZERODHA LINK</div>
  <div class="tab" onclick="switchTab('learn')">📚 LEARN</div>
</div>

<!-- ═══════════════ OHLC PANEL ═══════════════ -->
<div id="panel-ohlc" class="panel active">

  <div class="card">
    <div class="card-title">⚡ SELECT INDEX / INSTRUMENT</div>
    <div class="ticker-row">
      <div class="ticker-chip active" onclick="selectTicker(this,'BANKNIFTY')">BANKNIFTY</div>
      <div class="ticker-chip" onclick="selectTicker(this,'NIFTY')">NIFTY</div>
      <div class="ticker-chip" onclick="selectTicker(this,'FINNIFTY')">FINNIFTY</div>
      <div class="ticker-chip" onclick="selectTicker(this,'SENSEX')">SENSEX</div>
      <div class="ticker-chip" onclick="selectTicker(this,'MIDCPNIFTY')">MIDCAP</div>
    </div>
    <div class="input-grid">
      <div class="input-group">
        <label>STRIKE PRICE</label>
        <input class="inp" id="strike" type="number" placeholder="56000" value="56000">
      </div>
      <div class="input-group">
        <label>TYPE</label>
        <select class="inp" id="optType">
          <option value="PE">PUT (PE)</option>
          <option value="CE">CALL (CE)</option>
        </select>
      </div>
    </div>
    <div class="input-grid">
      <div class="input-group">
        <label>OPEN (₹)</label>
        <input class="inp" id="oOpen" type="number" placeholder="313" value="313">
      </div>
      <div class="input-group">
        <label>HIGH (₹)</label>
        <input class="inp" id="oHigh" type="number" placeholder="315" value="315">
      </div>
      <div class="input-group">
        <label>LOW (₹)</label>
        <input class="inp" id="oLow" type="number" placeholder="186.60" value="186.60">
      </div>
      <div class="input-group">
        <label>CLOSE (₹)</label>
        <input class="inp" id="oClose" type="number" placeholder="236.90" value="236.90">
      </div>
    </div>
    <div class="input-grid">
      <div class="input-group">
        <label>TODAY OPEN (₹)</label>
        <input class="inp" id="todayOpen" type="number" placeholder="321">
      </div>
      <div class="input-group">
        <label>LOT SIZE</label>
        <input class="inp" id="lotSize" type="number" placeholder="15" value="15">
      </div>
    </div>
    <button class="btn btn-primary" onclick="analyzeOHLC()">⚡ ANALYZE NOW</button>
  </div>

  <div class="loading" id="ohlcLoading">
    <div class="spinner"></div>
    <div class="loading-text">AI COMPUTING LEVELS...</div>
  </div>

  <div id="ohlcOutput">
    <!-- Signal Box -->
    <div class="signal-box" id="mainSignal">
      <div class="signal-main text-green" id="signalText">BUY PE</div>
      <div class="signal-sub" id="signalSub">BULLISH MOMENTUM • HIGH CONFIDENCE</div>
    </div>

    <!-- CE vs PE Probability -->
    <div class="card green">
      <div class="card-title">📊 CE vs PE PROBABILITY</div>
      <div class="stat-row">
        <div class="stat-label text-green">CE</div>
        <div class="stat-track"><div class="stat-fill" id="ceBar" style="background:var(--green);width:0%"></div></div>
        <div class="stat-pct text-green" id="cePct">0%</div>
      </div>
      <div class="stat-row">
        <div class="stat-label text-red">PE</div>
        <div class="stat-track"><div class="stat-fill" id="peBar" style="background:var(--red);width:0%"></div></div>
        <div class="stat-pct text-red" id="pePct">0%</div>
      </div>
      <div class="stat-row">
        <div class="stat-label text-gold">SIDEWAY</div>
        <div class="stat-track"><div class="stat-fill" id="sideBar" style="background:var(--gold);width:0%"></div></div>
        <div class="stat-pct text-gold" id="sidePct">0%</div>
      </div>
    </div>

    <!-- Camarilla Levels -->
    <div class="card">
      <div class="card-title">🎯 CAMARILLA PIVOT LEVELS</div>
      <div id="camarillaLevels"></div>
    </div>

    <!-- All Pivots -->
    <div class="card gold">
      <div class="card-title">📐 ALL PIVOT SYSTEMS</div>
      <div id="allPivots"></div>
    </div>

    <!-- Indicators -->
    <div class="card">
      <div class="card-title">📡 INDICATOR SIGNALS</div>
      <div id="indicatorSignals"></div>
    </div>

    <!-- Opening Scenarios -->
    <div class="card red">
      <div class="card-title">🗺️ ALL OPENING SCENARIOS</div>
      <div id="openingScenarios"></div>
    </div>

    <!-- Psychology -->
    <div class="card gold">
      <div class="card-title">🧠 MARKET PSYCHOLOGY</div>
      <div id="psychAnalysis"></div>
    </div>

    <!-- AI Deep Analysis -->
    <div class="card">
      <div class="card-title">🤖 AI DEEP ANALYSIS</div>
      <div class="loading" id="aiLoading"><div class="spinner"></div><div class="loading-text">CONSULTING AI...</div></div>
      <div class="ai-output" id="aiText" style="display:none"></div>
    </div>

    <div class="disclaimer">⚠️ EDUCATIONAL PURPOSE ONLY. NOT SEBI-REGISTERED ADVICE. OPTIONS TRADING INVOLVES SUBSTANTIAL RISK. ALWAYS USE STOP LOSSES. PAST ANALYSIS DOES NOT GUARANTEE FUTURE RESULTS.</div>
  </div>
</div>

<!-- ═══════════════ CHART SCANNER PANEL ═══════════════ -->
<div id="panel-chart" class="panel">
  <div class="card">
    <div class="card-title">📸 UPLOAD CHART SCREENSHOT</div>
    <div class="upload-zone" id="uploadZone" onclick="document.getElementById('chartFile').click()">
      <div class="upload-icon">📊</div>
      <div class="upload-text">TAP TO UPLOAD CHART<br><span style="font-size:10px;color:var(--dim)">BankNifty, Nifty, FinNifty, Any Option Chart</span></div>
      <img id="chartPreview" alt="Chart">
    </div>
    <input type="file" id="chartFile" accept="image/*" style="display:none" onchange="handleChartUpload(event)">
  </div>

  <div class="card" id="chartContextCard" style="display:none">
    <div class="card-title">⚙️ CHART CONTEXT (OPTIONAL)</div>
    <div class="input-grid">
      <div class="input-group">
        <label>INDEX</label>
        <select class="inp" id="chartIndex">
          <option>BANKNIFTY</option>
          <option>NIFTY</option>
          <option>FINNIFTY</option>
          <option>SENSEX</option>
        </select>
      </div>
      <div class="input-group">
        <label>TIMEFRAME</label>
        <select class="inp" id="chartTF">
          <option>15M</option>
          <option>5M</option>
          <option>1H</option>
          <option>DAILY</option>
        </select>
      </div>
    </div>
    <button class="btn btn-primary" onclick="scanChart()">🔍 SCAN & ANALYZE CHART</button>
  </div>

  <div class="loading" id="chartLoading">
    <div class="spinner"></div>
    <div class="loading-text">AI READING CHART...</div>
  </div>

  <div id="chartOutput">
    <div class="card green">
      <div class="card-title">🎯 AI CHART VERDICT</div>
      <div class="signal-box" style="margin-bottom:0">
        <div class="signal-main" id="chartSignalMain">--</div>
        <div class="signal-sub" id="chartSignalSub">Upload a chart to begin</div>
      </div>
    </div>
    <div class="card">
      <div class="card-title">📡 INDICATOR READINGS FROM CHART</div>
      <div id="chartIndicators"></div>
    </div>
    <div class="card red">
      <div class="card-title">🤖 AI FULL CHART ANALYSIS</div>
      <div class="ai-output" id="chartAiText"></div>
    </div>
    <div class="disclaimer">⚠️ AI image analysis is approximate. Always verify with live market data before trading.</div>
  </div>
</div>

<!-- ═══════════════ ZERODHA PANEL ═══════════════ -->
<div id="panel-zerodha" class="panel">
  <div class="card">
    <div class="card-title">🔗 ZERODHA KITE INTEGRATION</div>
    <div class="zerodha-info">
      <div style="font-size:13px;color:var(--accent);margin-bottom:12px;font-family:'Orbitron',sans-serif;font-size:11px;letter-spacing:2px;">HOW TO CONNECT ZERODHA</div>
      <div class="step-item">
        <div class="step-num">1</div>
        <div class="step-text">Go to <span class="step-code">kite.zerodha.com/api</span> → Create a new app → Get your <span class="step-code">API Key</span> and <span class="step-code">API Secret</span></div>
      </div>
      <div class="step-item">
        <div class="step-num">2</div>
        <div class="step-text">Enter your credentials below. Your keys are stored ONLY in your browser — never sent to any server except Zerodha's official API.</div>
      </div>
      <div class="step-item">
        <div class="step-num">3</div>
        <div class="step-text">After connecting, this app fetches LIVE option chain, OI, IV, and spot price automatically for analysis.</div>
      </div>
      <div class="step-item">
        <div class="step-num">4</div>
        <div class="step-text">⚠️ Zerodha KiteConnect API costs ₹2000/month for live data. Free for paper trading mode using delayed data.</div>
      </div>
    </div>
  </div>

  <div class="card">
    <div class="card-title">🔑 API CREDENTIALS</div>
    <div class="input-group mb8">
      <label>ZERODHA API KEY</label>
      <input class="inp" id="zApiKey" type="password" placeholder="Enter your API Key">
    </div>
    <div class="input-group mb8">
      <label>ZERODHA API SECRET</label>
      <input class="inp" id="zApiSecret" type="password" placeholder="Enter your API Secret">
    </div>
    <div class="input-group mb8">
      <label>ACCESS TOKEN (After Login)</label>
      <input class="inp" id="zAccessToken" type="password" placeholder="Generated after each login">
    </div>
    <button class="btn btn-primary mb8" onclick="saveZerodha()">💾 SAVE CREDENTIALS</button>
    <button class="btn btn-gold" onclick="testZerodha()">🧪 TEST CONNECTION</button>
  </div>

  <div class="card green">
    <div class="card-title">📊 LIVE DATA (AFTER CONNECTION)</div>
    <div id="liveDataSection">
      <div style="text-align:center;padding:20px;color:var(--dim);font-family:'Share Tech Mono',monospace;font-size:11px;">
        Connect Zerodha API to see<br>live option chain data here
      </div>
    </div>
  </div>

  <div class="card gold">
    <div class="card-title">⚡ AUTO-TRADE SETTINGS (PAPER MODE)</div>
    <div style="font-size:11px;color:var(--dim);font-family:'Share Tech Mono',monospace;line-height:1.8;margin-bottom:12px;">
      Paper trading mode — signals generated but NO real orders placed. Perfect for testing strategy before going live.
    </div>
    <div class="input-group mb8">
      <label>MAX CAPITAL PER TRADE (₹)</label>
      <input class="inp" id="maxCapital" type="number" placeholder="10000" value="10000">
    </div>
    <div class="input-group mb8">
      <label>MAX LOSS PER DAY (₹)</label>
      <input class="inp" id="maxLoss" type="number" placeholder="3000" value="3000">
    </div>
    <div class="input-group mb8">
      <label>TARGET % PER TRADE</label>
      <input class="inp" id="targetPct" type="number" placeholder="30" value="30">
    </div>
    <button class="btn btn-danger" onclick="savePaperSettings()">💾 SAVE SETTINGS</button>
  </div>

  <div class="disclaimer">⚠️ This app does NOT place real orders automatically. All trade execution must be done manually on Zerodha Kite. Auto-trading requires SEBI algo trading approval. Use at your own risk.</div>
</div>

<!-- ═══════════════ LEARN PANEL ═══════════════ -->
<div id="panel-learn" class="panel">
  <div class="card">
    <div class="card-title">📚 CAMARILLA FORMULA</div>
    <div class="ai-output" style="display:block;max-height:200px;">Range = High - Low

H4 = Close + (Range × 1.1/2)  ← SELL ZONE
H3 = Close + (Range × 1.1/4)  ← TARGET 2
H2 = Close + (Range × 1.1/6)  ← TARGET 1
H1 = Close + (Range × 1.1/12) ← SCALP T1
PP = (H+L+C) / 3              ← TREND DECIDER
L1 = Close - (Range × 1.1/12) ← SUPPORT 1
L2 = Close - (Range × 1.1/6)  ← SUPPORT 2
L3 = Close - (Range × 1.1/4)  ← DANGER
L4 = Close - (Range × 1.1/2)  ← PANIC ZONE</div>
  </div>

  <div class="card gold">
    <div class="card-title">🧠 5 GOLDEN RULES</div>
    <div id="goldenRules"></div>
  </div>

  <div class="card">
    <div class="card-title">📊 INDICATOR GUIDE</div>
    <div id="indicatorGuide"></div>
  </div>

  <div class="card red">
    <div class="card-title">🧠 PSYCHOLOGY RULES</div>
    <div id="psychRules"></div>
  </div>

  <div class="card green">
    <div class="card-title">🤖 ASK AI ANYTHING</div>
    <div class="input-group mb8">
      <label>YOUR TRADING QUESTION</label>
      <input class="inp" id="learnQ" type="text" placeholder="What is open interest? How to read ADX?">
    </div>
    <button class="btn btn-primary" onclick="askLearnAI()">🤖 ASK AI GURU</button>
    <div class="loading" id="learnLoading" style="margin-top:12px"><div class="spinner"></div><div class="loading-text">THINKING...</div></div>
    <div class="ai-output mt8" id="learnAnswer" style="display:none;max-height:300px;"></div>
  </div>
</div>

<script>
// ═══════════════════════════════════════════
// STATE
// ═══════════════════════════════════════════
let selectedTicker = 'BANKNIFTY';
let chartImageBase64 = null;

// ═══════════════════════════════════════════
// TAB SWITCHING
// ═══════════════════════════════════════════
function switchTab(tab) {
  document.querySelectorAll('.tab').forEach((t,i) => {
    const tabs = ['ohlc','chart','zerodha','learn'];
    t.classList.toggle('active', tabs[i] === tab);
  });
  document.querySelectorAll('.panel').forEach(p => p.classList.remove('active'));
  document.getElementById('panel-'+tab).classList.add('active');
  if(tab==='learn') renderLearnContent();
}

function selectTicker(el, ticker) {
  document.querySelectorAll('.ticker-chip').forEach(c => c.classList.remove('active'));
  el.classList.add('active');
  selectedTicker = ticker;
  const lotSizes = {BANKNIFTY:15,NIFTY:25,FINNIFTY:40,SENSEX:10,MIDCPNIFTY:50};
  document.getElementById('lotSize').value = lotSizes[ticker]||15;
}

// ═══════════════════════════════════════════
// CAMARILLA CALCULATION ENGINE
// ═══════════════════════════════════════════
function calcCamarilla(H,L,C) {
  const R = H - L;
  return {
    H4: +(C + R*1.1/2).toFixed(2),
    H3: +(C + R*1.1/4).toFixed(2),
    H2: +(C + R*1.1/6).toFixed(2),
    H1: +(C + R*1.1/12).toFixed(2),
    PP: +((H+L+C)/3).toFixed(2),
    L1: +(C - R*1.1/12).toFixed(2),
    L2: +(C - R*1.1/6).toFixed(2),
    L3: +(C - R*1.1/4).toFixed(2),
    L4: +(C - R*1.1/2).toFixed(2),
    range: +R.toFixed(2)
  };
}

function calcStandardPivot(H,L,C) {
  const PP = +((H+L+C)/3).toFixed(2);
  return {
    PP,
    R1: +(2*PP - L).toFixed(2),
    R2: +(PP + H - L).toFixed(2),
    R3: +(H + 2*(PP - L)).toFixed(2),
    S1: +(2*PP - H).toFixed(2),
    S2: +(PP - H + L).toFixed(2),
    S3: +(L - 2*(H - PP)).toFixed(2),
  };
}

function calcFibPivot(H,L,C) {
  const PP = +((H+L+C)/3).toFixed(2);
  const R = H-L;
  return {
    PP,
    R1: +(PP + 0.382*R).toFixed(2),
    R2: +(PP + 0.618*R).toFixed(2),
    R3: +(PP + 1.000*R).toFixed(2),
    S1: +(PP - 0.382*R).toFixed(2),
    S2: +(PP - 0.618*R).toFixed(2),
    S3: +(PP - 1.000*R).toFixed(2),
  };
}

function calcWoodiesPivot(H,L,C,O) {
  const PP = +((H+L+2*C)/4).toFixed(2);
  return {
    PP,
    R1: +(2*PP - L).toFixed(2),
    R2: +(PP + H - L).toFixed(2),
    S1: +(2*PP - H).toFixed(2),
    S2: +(PP - H + L).toFixed(2),
  };
}

function calcDemarkPivot(H,L,C,O) {
  let X;
  if(C < O) X = H + 2*L + C;
  else if(C > O) X = 2*H + L + C;
  else X = H + L + 2*C;
  const PP = +(X/4).toFixed(2);
  return {
    PP,
    R1: +(X/2 - L).toFixed(2),
    S1: +(X/2 - H).toFixed(2),
  };
}

// ═══════════════════════════════════════════
// TECHNICAL INDICATORS (Approximation)
// ═══════════════════════════════════════════
function estimateIndicators(H,L,C,O) {
  const R = H-L;
  const mid = (H+L)/2;
  const closeVsMid = (C - L) / R; // 0=at low, 1=at high

  // RSI approximation based on close position
  const rsiApprox = +(30 + closeVsMid * 40).toFixed(0);

  // Candle body analysis
  const bodySize = Math.abs(C-O);
  const upperWick = H - Math.max(C,O);
  const lowerWick = Math.min(C,O) - L;
  const isBullish = C > O;

  // MACD signal (based on close vs pivot)
  const pp = (H+L+C)/3;
  const macdBull = C > pp;

  // ADX approximation
  const adxStrength = R > (C*0.1) ? 'STRONG' : R > (C*0.05) ? 'MODERATE' : 'WEAK';

  // Bollinger position
  const bbMid = (H+L+C)/3;
  const bbPos = C > bbMid ? 'UPPER_HALF' : 'LOWER_HALF';

  // Volume/momentum proxy
  const momentumBull = lowerWick > upperWick; // long lower wick = bullish

  return {
    rsi: rsiApprox,
    rsiSignal: rsiApprox > 60 ? 'OVERBOUGHT' : rsiApprox < 40 ? 'OVERSOLD' : 'NEUTRAL',
    macd: macdBull ? 'BULLISH' : 'BEARISH',
    adx: adxStrength,
    bbPos,
    momentum: momentumBull ? 'BULLISH' : 'BEARISH',
    candleType: isBullish ? 'BULLISH CANDLE' : 'BEARISH CANDLE',
    upperWick: +upperWick.toFixed(2),
    lowerWick: +lowerWick.toFixed(2),
    bodyPct: +((bodySize/R)*100).toFixed(1),
    closeVsMid: +closeVsMid.toFixed(2)
  };
}

// ═══════════════════════════════════════════
// MAIN ANALYZE FUNCTION
// ═══════════════════════════════════════════
function analyzeOHLC() {
  const H = parseFloat(document.getElementById('oHigh').value);
  const L = parseFloat(document.getElementById('oLow').value);
  const C = parseFloat(document.getElementById('oClose').value);
  const O = parseFloat(document.getElementById('oOpen').value);
  const todayOpen = parseFloat(document.getElementById('todayOpen').value) || null;
  const optType = document.getElementById('optType').value;
  const lotSize = parseInt(document.getElementById('lotSize').value)||15;
  const strike = document.getElementById('strike').value;

  if(!H||!L||!C||!O||H<L) { alert('Please enter valid OHLC values'); return; }

  document.getElementById('ohlcLoading').classList.add('show');
  document.getElementById('ohlcOutput').style.display='none';

  setTimeout(() => {
    document.getElementById('ohlcLoading').classList.remove('show');
    document.getElementById('ohlcOutput').classList.add('show');
    document.getElementById('ohlcOutput').style.display='block';

    const cam = calcCamarilla(H,L,C);
    const std = calcStandardPivot(H,L,C);
    const fib = calcFibPivot(H,L,C);
    const woo = calcWoodiesPivot(H,L,C,O);
    const dem = calcDemarkPivot(H,L,C,O);
    const ind = estimateIndicators(H,L,C,O);

    renderSignal(cam, ind, optType, todayOpen, C);
    renderCEPEProb(cam, ind, optType, C, todayOpen);
    renderCamarillaLevels(cam, C, todayOpen);
    renderAllPivots(std, fib, woo, dem);
    renderIndicators(ind);
    renderOpeningScenarios(cam, C, lotSize, todayOpen);
    renderPsychology(cam, ind, C, H, L, O, optType);
    callAIAnalysis(H,L,C,O,cam,ind,optType,strike,selectedTicker,todayOpen);

    setTimeout(()=>{ animateBars(); }, 100);
  }, 800);
}

function renderSignal(cam, ind, optType, todayOpen, C) {
  let signals = 0, total = 5;
  if(ind.momentum === 'BULLISH') signals++;
  if(ind.macd === 'BULLISH') signals++;
  if(ind.rsiSignal === 'OVERSOLD') signals++;
  if(C > cam.PP) signals++;
  if(todayOpen && todayOpen > C) signals++;

  const bullPct = Math.round((signals/total)*100);
  const bearPct = 100 - bullPct;
  const strong = bullPct >= 60;

  document.getElementById('signalText').textContent = strong ? `BUY ${optType}` : `AVOID / WAIT`;
  document.getElementById('signalText').className = `signal-main ${strong?'text-green':'text-gold'}`;
  document.getElementById('signalSub').textContent = `${bullPct}% BULLISH SIGNALS • ${bearPct}% BEARISH`;

  const box = document.getElementById('mainSignal');
  box.style.borderColor = strong ? 'rgba(0,255,136,0.3)' : 'rgba(255,184,0,0.3)';
  box.style.boxShadow = strong ? '0 0 30px rgba(0,255,136,0.1)' : '0 0 30px rgba(255,184,0,0.1)';
}

function renderCEPEProb(cam, ind, optType, C, todayOpen) {
  let peBullScore = 0;
  if(ind.momentum==='BULLISH') peBullScore += 20;
  if(ind.macd==='BULLISH') peBullScore += 20;
  if(C < cam.PP) peBullScore += 15;
  if(ind.lowerWick > ind.upperWick) peBullScore += 20;
  if(ind.rsiSignal==='OVERSOLD') peBullScore += 15;
  if(todayOpen && todayOpen > C) peBullScore += 10;

  peBullScore = Math.min(85, peBullScore);
  const cePct = Math.max(5, 100 - peBullScore - 10);
  const sidePct = Math.max(5, 100 - peBullScore - cePct);
  const total = peBullScore + cePct + sidePct;
  const peNorm = Math.round(peBullScore/total*100);
  const ceNorm = Math.round(cePct/total*100);
  const sideNorm = 100 - peNorm - ceNorm;

  document.getElementById('pePct').textContent = peNorm+'%';
  document.getElementById('cePct').textContent = ceNorm+'%';
  document.getElementById('sidePct').textContent = sideNorm+'%';
  document.getElementById('peBar').dataset.width = peNorm;
  document.getElementById('ceBar').dataset.width = ceNorm;
  document.getElementById('sideBar').dataset.width = sideNorm;
}

function animateBars() {
  document.querySelectorAll('[data-width]').forEach(el => {
    el.style.width = el.dataset.width + '%';
  });
}

function renderCamarillaLevels(cam, C, todayOpen) {
  const current = todayOpen || C;
  const levels = [
    { label:'H4', price:cam.H4, color:'#ff3e6c', action:'SELL ZONE', barColor:'#ff3e6c', barPct:95 },
    { label:'H3', price:cam.H3, color:'#ff8c42', action:'TARGET 2', barColor:'#ff8c42', barPct:75 },
    { label:'H2', price:cam.H2, color:'#ffb800', action:'TARGET 1', barColor:'#ffb800', barPct:60 },
    { label:'H1', price:cam.H1, color:'#88ff00', action:'SCALP T1', barColor:'#88ff00', barPct:50 },
    { label:'PP', price:cam.PP, color:'#00f5ff', action:'DECIDER', barColor:'#00f5ff', barPct:45 },
    { label:'L1', price:cam.L1, color:'#88ff00', action:'SUPPORT1', barColor:'#88ff00', barPct:38 },
    { label:'L2', price:cam.L2, color:'#ffb800', action:'SUPPORT2', barColor:'#ffb800', barPct:28 },
    { label:'L3', price:cam.L3, color:'#ff8c42', action:'DANGER', barColor:'#ff8c42', barPct:18 },
    { label:'L4', price:cam.L4, color:'#ff3e6c', action:'PANIC', barColor:'#ff3e6c', barPct:8 },
  ];

  let html = '';
  levels.forEach(lv => {
    const isCurrent = Math.abs(current - lv.price) < (cam.H4 - cam.L4) * 0.08;
    html += `<div class="level-row" style="${isCurrent?'background:rgba(0,245,255,0.06);border-radius:6px;':''} ">
      <div class="level-label" style="color:${lv.color}">${lv.label}</div>
      <div class="level-bar-wrap"><div class="level-bar" style="background:${lv.barColor};width:${lv.barPct}%"></div></div>
      <div class="level-price" style="color:${lv.color}">₹${lv.price}</div>
      <div class="level-action" style="background:${lv.color}22;color:${lv.color};font-size:9px;padding:2px 4px;border-radius:4px;font-family:'Share Tech Mono',monospace;letter-spacing:0.5px">${lv.action}${isCurrent?' ◄':''}</div>
    </div>`;
  });

  // Trade plan
  const entryZone = current < cam.PP ? `₹${cam.L1}–₹${cam.PP}` : `₹${cam.PP}–₹${cam.H1}`;
  const sl = current < cam.PP ? `₹${cam.L2}` : `₹${cam.L1}`;
  const t1 = cam.H2, t2 = cam.H3, t3 = cam.H4;
  const risk = +(current - parseFloat(sl.replace('₹',''))).toFixed(2);
  const reward = +(t2 - current).toFixed(2);
  const rr = risk > 0 ? (reward/risk).toFixed(1) : '--';

  html += `<div style="margin-top:12px;padding:12px;background:var(--bg3);border-radius:8px;border:1px solid rgba(0,245,255,0.1)">
    <div style="font-family:'Orbitron',sans-serif;font-size:9px;letter-spacing:2px;color:var(--accent);margin-bottom:8px">TRADE PLAN</div>
    <table style="width:100%;font-family:'Share Tech Mono',monospace;font-size:11px;">
      <tr><td style="color:var(--dim);padding:3px 0">ENTRY ZONE</td><td style="color:var(--accent);text-align:right">${entryZone}</td></tr>
      <tr><td style="color:var(--dim);padding:3px 0">STOP LOSS</td><td style="color:var(--red);text-align:right">${sl}</td></tr>
      <tr><td style="color:var(--dim);padding:3px 0">TARGET 1</td><td style="color:var(--green);text-align:right">₹${t1}</td></tr>
      <tr><td style="color:var(--dim);padding:3px 0">TARGET 2</td><td style="color:var(--green);text-align:right">₹${t2}</td></tr>
      <tr><td style="color:var(--dim);padding:3px 0">TARGET 3</td><td style="color:var(--green);text-align:right">₹${t3}</td></tr>
      <tr><td style="color:var(--dim);padding:3px 0">RISK:REWARD</td><td style="color:var(--gold);text-align:right">1:${rr}</td></tr>
    </table>
  </div>`;

  document.getElementById('camarillaLevels').innerHTML = html;
}

function renderAllPivots(std, fib, woo, dem) {
  const systems = [
    { name:'STANDARD', data:std, color:var_color('accent') },
    { name:'FIBONACCI', data:fib, color:var_color('gold') },
    { name:"WOODIE'S", data:woo, color:'#88ff00' },
    { name:"DeMARK", data:dem, color:'#ff8c42' },
  ];
  let html = '';
  systems.forEach(s => {
    html += `<div style="margin-bottom:10px">
      <div style="font-family:'Share Tech Mono',monospace;font-size:9px;letter-spacing:2px;color:${s.color};margin-bottom:4px">${s.name} PIVOT</div>
      <div style="display:flex;flex-wrap:wrap;gap:4px">`;
    Object.entries(s.data).forEach(([k,v]) => {
      const isR = k.startsWith('R');
      const isS = k.startsWith('S');
      const bg = isR ? 'rgba(255,62,108,0.12)' : isS ? 'rgba(0,255,136,0.12)' : 'rgba(0,245,255,0.12)';
      const cl = isR ? '#ff3e6c' : isS ? '#00ff88' : '#00f5ff';
      html += `<div style="background:${bg};color:${cl};padding:4px 8px;border-radius:4px;font-family:'Share Tech Mono',monospace;font-size:10px"><span style="opacity:0.6">${k}:</span> ₹${v}</div>`;
    });
    html += `</div></div>`;
  });
  document.getElementById('allPivots').innerHTML = html;
}

function var_color(name) {
  const map={accent:'#00f5ff',gold:'#ffb800',green:'#00ff88',red:'#ff3e6c'};
  return map[name]||'#fff';
}

function renderIndicators(ind) {
  const items = [
    { name:'RSI (14)', value:`${ind.rsi} — ${ind.rsiSignal}`, signal:ind.rsiSignal==='OVERSOLD'?'bull':ind.rsiSignal==='OVERBOUGHT'?'bear':'neutral' },
    { name:'MACD', value:ind.macd, signal:ind.macd==='BULLISH'?'bull':'bear' },
    { name:'ADX Strength', value:ind.adx, signal:'neutral' },
    { name:'Bollinger', value:ind.bbPos==='UPPER_HALF'?'ABOVE MID':'BELOW MID', signal:ind.bbPos==='UPPER_HALF'?'bull':'bear' },
    { name:'Momentum', value:ind.momentum, signal:ind.momentum==='BULLISH'?'bull':'bear' },
    { name:'Candle Type', value:ind.candleType, signal:ind.candleType.includes('BULL')?'bull':'bear' },
    { name:'Upper Wick', value:`₹${ind.upperWick}`, signal:'neutral' },
    { name:'Lower Wick', value:`₹${ind.lowerWick}`, signal:ind.lowerWick>ind.upperWick?'bull':'bear' },
    { name:'Body %', value:`${ind.bodyPct}%`, signal:'neutral' },
    { name:'Close vs Mid', value:ind.closeVsMid>0.5?'ABOVE MIDPOINT':'BELOW MIDPOINT', signal:ind.closeVsMid>0.5?'bull':'bear' },
  ];
  let html = '';
  items.forEach(item => {
    html += `<div class="gauge-row">
      <div class="gauge-name">${item.name}</div>
      <div class="gauge-signal sig-${item.signal}">${item.value}</div>
    </div>`;
  });
  document.getElementById('indicatorSignals').innerHTML = html;
}

function renderOpeningScenarios(cam, C, lotSize, todayOpen) {
  const scenarios = [
    {
      type:'bull', label:'GAP UP — OPENS ABOVE H3',
      openRange:`₹${cam.H3}+`,
      entry:`₹${cam.H3+5}–₹${cam.H2}`,
      sl:`₹${cam.PP}`,
      t1:`₹${cam.H3+20}`, t2:`₹${cam.H4}`, t3:`₹${+(cam.H4*1.05).toFixed(0)}`,
      note:'Gap up = BankNifty crashed. Premium inflated. Wait for pullback to H3 before buying.',
      risk: +(cam.H3+5 - cam.PP).toFixed(0),
      reward: +(cam.H4 - cam.H3 - 5).toFixed(0)
    },
    {
      type:'neutral', label:'FLAT OPEN — NEAR PP',
      openRange:`₹${cam.L1}–₹${cam.H1}`,
      entry:`₹${+(cam.PP+2).toFixed(0)} (after PP breakout)`,
      sl:`₹${cam.L1}`,
      t1:`₹${cam.H2}`, t2:`₹${cam.H3}`, t3:`₹${cam.H4}`,
      note:'Wait for 15 minutes. Trade breakout above PP with volume confirmation. First 15 min = trap time.',
      risk: +(cam.PP+2 - cam.L1).toFixed(0),
      reward: +(cam.H3 - cam.PP - 2).toFixed(0)
    },
    {
      type:'bear', label:'GAP DOWN — OPENS NEAR L2',
      openRange:`₹${cam.L3}–₹${cam.L1}`,
      entry:`₹${+(cam.L2+3).toFixed(0)} (confirm bounce)`,
      sl:`₹${cam.L3}`,
      t1:`₹${cam.L1}`, t2:`₹${cam.PP}`, t3:`₹${cam.H2}`,
      note:'Best risk:reward setup. Gap down creates fear = smart money accumulates. Buy only with L2 bounce confirmation.',
      risk: +(cam.L2+3 - cam.L3).toFixed(0),
      reward: +(cam.PP - cam.L2 - 3).toFixed(0)
    },
    {
      type:'bear', label:'EXTREME GAP DOWN — BELOW L4',
      openRange:`Below ₹${cam.L4}`,
      entry:'DO NOT BUY',
      sl:'N/A', t1:'N/A', t2:'N/A', t3:'N/A',
      note:'Breakdown zone. BankNifty in strong bull run. Exit all PE positions. Capital preservation first.',
      risk: 0, reward: 0
    },
    {
      type:'bull', label:'EXTREME GAP UP — ABOVE H4',
      openRange:`Above ₹${cam.H4}`,
      entry:'BOOK PROFITS ONLY',
      sl:`₹${cam.H3}`, t1:'N/A', t2:'N/A', t3:'N/A',
      note:'If holding from lower — book full profit! 90% probability of reversal at H4. DO NOT buy new position here.',
      risk: 0, reward: 0
    },
  ];

  // If today's open is provided, highlight the matching scenario
  let activeScenario = null;
  if(todayOpen) {
    if(todayOpen > cam.H4) activeScenario = 4;
    else if(todayOpen > cam.H3) activeScenario = 0;
    else if(todayOpen > cam.L1) activeScenario = 1;
    else if(todayOpen > cam.L3) activeScenario = 2;
    else activeScenario = 3;
  }

  let html = '';
  scenarios.forEach((s,i) => {
    const rr = s.risk > 0 ? (s.reward/s.risk).toFixed(1) : '--';
    const highlight = activeScenario===i ? 'border:1px solid var(--accent);box-shadow:var(--glow);' : '';
    html += `<div class="scenario ${s.type}" style="${highlight}">
      <div class="scenario-title" style="color:${s.type==='bull'?'var(--green)':s.type==='bear'?'var(--red)':'var(--gold)'}">
        ${s.type==='bull'?'📈':s.type==='bear'?'📉':'⚖️'} ${s.label} ${activeScenario===i?'◄ TODAY':''}
      </div>
      <div class="scenario-grid">
        <div class="sg-item"><div class="sg-label">OPEN RANGE</div><div class="sg-value text-accent">${s.openRange}</div></div>
        <div class="sg-item"><div class="sg-label">ENTRY</div><div class="sg-value text-green">${s.entry}</div></div>
        <div class="sg-item"><div class="sg-label">STOP LOSS</div><div class="sg-value text-red">${s.sl}</div></div>
        <div class="sg-item"><div class="sg-label">R:R RATIO</div><div class="sg-value text-gold">1:${rr}</div></div>
        <div class="sg-item"><div class="sg-label">TARGET 1</div><div class="sg-value text-green">${s.t1}</div></div>
        <div class="sg-item"><div class="sg-label">TARGET 2</div><div class="sg-value text-green">${s.t2}</div></div>
      </div>
      <div style="margin-top:8px;font-size:11px;color:var(--dim);line-height:1.6;font-family:'Share Tech Mono',monospace;">${s.note}</div>
    </div>`;
  });
  document.getElementById('openingScenarios').innerHTML = html;
}

function renderPsychology(cam, ind, C, H, L, O, optType) {
  const isLongUpperWick = ind.upperWick > (H-L)*0.3;
  const isLongLowerWick = ind.lowerWick > (H-L)*0.3;
  const closedNearHigh = (H-C) < (H-L)*0.2;
  const closedNearLow = (C-L) < (H-L)*0.2;

  const patterns = [];
  if(isLongUpperWick && !isLongLowerWick) patterns.push({p:'SHOOTING STAR / BEARISH REJECTION',d:'Price rejected at highs. Sellers are strong. Avoid buying near the high. Expect pullback.',c:'red'});
  if(isLongLowerWick && !isLongUpperWick) patterns.push({p:'HAMMER / BULLISH REVERSAL',d:'Price rejected at lows. Buyers stepped in strongly. Good sign for longs. Buy near the low.',c:'green'});
  if(isLongUpperWick && isLongLowerWick) patterns.push({p:'DOJI / SPINNING TOP',d:'Market indecision. Neither bulls nor bears in control. Wait for next candle direction before trading.',c:'gold'});
  if(closedNearHigh) patterns.push({p:'BULLISH CLOSE — STRONG BUYING',d:'Close near high = buyers in control at end of day. Momentum likely to continue next session.',c:'green'});
  if(closedNearLow) patterns.push({p:'BEARISH CLOSE — STRONG SELLING',d:'Close near low = sellers dominating. Next session likely to see continuation of selling.',c:'red'});

  const rules = [
    { icon:'⏰', rule:'9:15–9:30 = Trap Zone', desc:'First 15 minutes is institutional trap. Retail traders get caught by false moves. WAIT.' },
    { icon:'📊', rule:'Volume Confirms Move', desc:'A breakout without volume = false signal. Always check if volume is above average.' },
    { icon:'😨', rule:'Fear = Opportunity', desc:'When everyone is selling PE (gap down), smart money is buying. Buy fear with support confirmation.' },
    { icon:'🤑', rule:'Greed = Danger', desc:'When PE gaps up above H4, everyone wants to buy. Smart money is selling. Book profits, not adding.' },
    { icon:'🎯', rule:'1:2 R:R Minimum', desc:'Never trade below 1:2 risk reward. If you risk ₹20, target must be ₹40+. Non-negotiable.' },
    { icon:'✂️', rule:'Cut Losses Fast', desc:'A small loss today saves a big loss tomorrow. No averaging down in options — time decay kills.' },
  ];

  let html = `<div style="margin-bottom:12px">
    <div class="result-title">CANDLE PSYCHOLOGY</div>`;
  if(patterns.length===0) {
    html += `<div style="color:var(--dim);font-size:11px;font-family:'Share Tech Mono',monospace">NORMAL CANDLE — No extreme pattern detected</div>`;
  }
  patterns.forEach(p => {
    html += `<div style="padding:8px;background:rgba(${p.c==='red'?'255,62,108':p.c==='green'?'0,255,136':'255,184,0'},0.08);border-radius:6px;margin-bottom:6px;border-left:2px solid var(--${p.c==='gold'?'gold':p.c})">
      <div style="font-size:11px;font-weight:700;color:var(--${p.c==='gold'?'gold':p.c});margin-bottom:2px">${p.p}</div>
      <div style="font-size:10px;color:var(--dim);font-family:'Share Tech Mono',monospace">${p.d}</div>
    </div>`;
  });
  html += `</div><div class="result-title">GOLDEN PSYCHOLOGY RULES</div>`;
  rules.forEach(r => {
    html += `<div style="display:flex;gap:10px;padding:8px 0;border-bottom:1px solid var(--border)">
      <div style="font-size:18px;flex-shrink:0">${r.icon}</div>
      <div>
        <div style="font-size:12px;font-weight:700;margin-bottom:2px">${r.rule}</div>
        <div style="font-size:10px;color:var(--dim);font-family:'Share Tech Mono',monospace;line-height:1.5">${r.desc}</div>
      </div>
    </div>`;
  });

  document.getElementById('psychAnalysis').innerHTML = html;
}

// ═══════════════════════════════════════════
// AI API CALL
// ═══════════════════════════════════════════
async function callAIAnalysis(H,L,C,O,cam,ind,optType,strike,ticker,todayOpen) {
  document.getElementById('aiLoading').classList.add('show');
  document.getElementById('aiText').style.display = 'none';

  const prompt = `You are an expert Indian options trader and technical analyst. Analyze this option:

INSTRUMENT: ${ticker} ${strike} ${optType}
OHLC: Open=₹${O}, High=₹${H}, Low=₹${L}, Close=₹${C}
${todayOpen ? `TODAY'S OPEN: ₹${todayOpen}` : ''}

CAMARILLA LEVELS:
H4=₹${cam.H4}, H3=₹${cam.H3}, H2=₹${cam.H2}, H1=₹${cam.H1}
PP=₹${cam.PP}
L1=₹${cam.L1}, L2=₹${cam.L2}, L3=₹${cam.L3}, L4=₹${cam.L4}

INDICATORS: RSI≈${ind.rsi}(${ind.rsiSignal}), MACD=${ind.macd}, Momentum=${ind.momentum}, Candle=${ind.candleType}

Provide a comprehensive analysis in this exact format:

📊 MARKET BIAS: [BULLISH/BEARISH/NEUTRAL] with confidence %

🎯 IDEAL ENTRY: ₹___ to ₹___
🛑 STOP LOSS: ₹___ (reason)
🎯 TARGET 1: ₹___ (probability %)
🎯 TARGET 2: ₹___ (probability %)
🎯 TARGET 3: ₹___ (probability %)

⚖️ RISK:REWARD: 1:___

${todayOpen ? `📍 TODAY OPEN ANALYSIS (₹${todayOpen}):
- Zone: [which Camarilla zone]
- Strategy: [specific action]
- Key observation:` : ''}

🧠 PSYCHOLOGY INSIGHT:
[2-3 sentences on market psychology for this setup]

⚠️ RISK FACTORS:
[2-3 key risks to this trade]

💡 SMART MONEY ANALYSIS:
[What institutional traders are likely doing at these levels]

Keep analysis sharp, specific with ₹ values. No generic advice.`;

  try {
    const res = await fetch('https://api.anthropic.com/v1/messages', {
      method:'POST',
      headers:{'Content-Type':'application/json'},
      body: JSON.stringify({
        model:'claude-sonnet-4-20250514',
        max_tokens:1000,
        messages:[{role:'user',content:prompt}]
      })
    });
    const data = await res.json();
    const text = data.content?.map(b=>b.text||'').join('') || 'Analysis unavailable';
    document.getElementById('aiText').textContent = text;
    document.getElementById('aiText').style.display = 'block';
  } catch(e) {
    document.getElementById('aiText').textContent = '⚠️ AI analysis unavailable. Check connection.\n\nUse the calculated Camarilla levels above for your trade plan.';
    document.getElementById('aiText').style.display = 'block';
  }
  document.getElementById('aiLoading').classList.remove('show');
}

// ═══════════════════════════════════════════
// CHART SCANNER
// ═══════════════════════════════════════════
function handleChartUpload(e) {
  const file = e.target.files[0];
  if(!file) return;
  const reader = new FileReader();
  reader.onload = (ev) => {
    chartImageBase64 = ev.target.result.split(',')[1];
    const preview = document.getElementById('chartPreview');
    preview.src = ev.target.result;
    preview.style.display = 'block';
    document.getElementById('chartContextCard').style.display = 'block';
    document.getElementById('uploadZone').style.borderColor = 'var(--green)';
  };
  reader.readAsDataURL(file);
}

function setupDragDrop() {
  const zone = document.getElementById('uploadZone');
  zone.addEventListener('dragover', e => { e.preventDefault(); zone.classList.add('drag'); });
  zone.addEventListener('dragleave', () => zone.classList.remove('drag'));
  zone.addEventListener('drop', e => {
    e.preventDefault();
    zone.classList.remove('drag');
    const file = e.dataTransfer.files[0];
    if(file && file.type.startsWith('image/')) {
      const dt = new DataTransfer();
      dt.items.add(file);
      document.getElementById('chartFile').files = dt.files;
      handleChartUpload({target:{files:[file]}});
    }
  });
}

async function scanChart() {
  if(!chartImageBase64) { alert('Please upload a chart first'); return; }
  const idx = document.getElementById('chartIndex').value;
  const tf = document.getElementById('chartTF').value;

  document.getElementById('chartLoading').classList.add('show');
  document.getElementById('chartOutput').style.display = 'none';

  const prompt = `You are an expert Indian options market technical analyst. Analyze this ${idx} ${tf} chart screenshot.

Provide your analysis in this EXACT format:

📊 CHART VERDICT: BUY CE / BUY PE / AVOID / WAIT
CONFIDENCE: ___%

CE PROBABILITY: ___%
PE PROBABILITY: ___%
SIDEWAYS PROBABILITY: ___%

📡 INDICATOR READINGS:
- ADX: [value/trend if visible] → [STRONG/WEAK TREND]
- MACD: [reading] → [BULLISH/BEARISH/CROSSOVER]
- RSI: [value if visible] → [OVERBOUGHT/OVERSOLD/NEUTRAL]
- Awesome Oscillator: [reading] → [signal]
- Pring KST: [reading if visible] → [signal]
- Candle Pattern: [what you see]
- Trend: [UP/DOWN/SIDEWAYS]
- Support: ₹___ (approximate)
- Resistance: ₹___ (approximate)

🎯 TRADE PLAN:
Entry: ₹___ to ₹___
Stop Loss: ₹___
Target 1: ₹___
Target 2: ₹___
Target 3: ₹___
Risk:Reward: 1:___

🧠 KEY OBSERVATION:
[Most important thing you see on this chart in 2-3 sentences]

⚠️ WARNING SIGNS:
[Any concerning signals on the chart]

Be specific with price levels if visible on chart. If levels are not clearly visible, give approximate zones.`;

  try {
    const res = await fetch('https://api.anthropic.com/v1/messages', {
      method:'POST',
      headers:{'Content-Type':'application/json'},
      body: JSON.stringify({
        model:'claude-sonnet-4-20250514',
        max_tokens:1200,
        messages:[{
          role:'user',
          content:[
            {type:'image',source:{type:'base64',media_type:'image/jpeg',data:chartImageBase64}},
            {type:'text',text:prompt}
          ]
        }]
      })
    });
    const data = await res.json();
    const text = data.content?.map(b=>b.text||'').join('') || '';

    document.getElementById('chartLoading').classList.remove('show');
    document.getElementById('chartOutput').style.display = 'block';

    // Parse signal
    const verdictMatch = text.match(/CHART VERDICT:\s*(.+)/i);
    const verdict = verdictMatch ? verdictMatch[1].trim() : 'ANALYZING';
    const isBuyCE = verdict.toUpperCase().includes('CE');
    const isBuyPE = verdict.toUpperCase().includes('PE');

    document.getElementById('chartSignalMain').textContent = verdict;
    document.getElementById('chartSignalMain').className = `signal-main ${isBuyCE?'text-green':isBuyPE?'text-red':'text-gold'}`;

    const confMatch = text.match(/CONFIDENCE:\s*(\d+)/i);
    document.getElementById('chartSignalSub').textContent = confMatch ? `CONFIDENCE: ${confMatch[1]}%` : 'AI ANALYSIS COMPLETE';

    // Render indicator table
    const indicators = ['ADX','MACD','RSI','Awesome Oscillator','Pring KST','Candle Pattern','Trend','Support','Resistance'];
    let indHtml = '';
    indicators.forEach(name => {
      const re = new RegExp(`${name}[:\\s]+([^\\n]+)`, 'i');
      const match = text.match(re);
      if(match) {
        const val = match[1].trim();
        const isBull = val.toLowerCase().includes('bull')||val.toLowerCase().includes('buy')||val.toLowerCase().includes('up')||val.toLowerCase().includes('golden');
        const isBear = val.toLowerCase().includes('bear')||val.toLowerCase().includes('sell')||val.toLowerCase().includes('down')||val.toLowerCase().includes('dead');
        indHtml += `<div class="gauge-row">
          <div class="gauge-name">${name}</div>
          <div class="gauge-signal ${isBull?'sig-bull':isBear?'sig-bear':'sig-neutral'}" style="max-width:180px;text-align:right;font-size:9px">${val.substring(0,50)}</div>
        </div>`;
      }
    });
    document.getElementById('chartIndicators').innerHTML = indHtml || '<div style="color:var(--dim);font-family:Share Tech Mono,monospace;font-size:11px">See full analysis below</div>';
    document.getElementById('chartAiText').textContent = text;

  } catch(e) {
    document.getElementById('chartLoading').classList.remove('show');
    document.getElementById('chartOutput').style.display = 'block';
    document.getElementById('chartAiText').textContent = '⚠️ Could not analyze chart. Please check your connection.';
  }
}

// ═══════════════════════════════════════════
// ZERODHA
// ═══════════════════════════════════════════
function saveZerodha() {
  const key = document.getElementById('zApiKey').value;
  const secret = document.getElementById('zApiSecret').value;
  const token = document.getElementById('zAccessToken').value;
  if(!key||!secret) { alert('Please enter API Key and Secret'); return; }
  localStorage.setItem('z_api_key', key);
  localStorage.setItem('z_api_secret', secret);
  if(token) localStorage.setItem('z_access_token', token);
  alert('✅ Credentials saved in browser! Ready to connect.');
}

function testZerodha() {
  const key = localStorage.getItem('z_api_key');
  if(!key) { alert('Please save credentials first'); return; }
  document.getElementById('liveDataSection').innerHTML = `
    <div style="padding:16px;text-align:center">
      <div style="color:var(--gold);font-family:'Share Tech Mono',monospace;font-size:11px;margin-bottom:8px">
        ⚠️ ZERODHA KITE API REQUIRES:
      </div>
      <div style="color:var(--dim);font-size:11px;font-family:'Share Tech Mono',monospace;line-height:2;text-align:left">
        1. Active KiteConnect subscription (₹2000/mo)<br>
        2. Daily login at kite.zerodha.com/api/login<br>
        3. Fresh access token generated each session<br>
        4. CORS proxy for browser requests<br><br>
        <span style="color:var(--green)">✅ Your API key is saved</span><br>
        <span style="color:var(--accent)">📱 For live data: Use Zerodha Kite app directly + enter OHLC in Analyzer tab</span>
      </div>
    </div>`;
}

function savePaperSettings() {
  const cap = document.getElementById('maxCapital').value;
  const loss = document.getElementById('maxLoss').value;
  const tgt = document.getElementById('targetPct').value;
  localStorage.setItem('paper_settings', JSON.stringify({cap,loss,tgt}));
  alert('✅ Paper trading settings saved!');
}

// ═══════════════════════════════════════════
// LEARN TAB
// ═══════════════════════════════════════════
function renderLearnContent() {
  const rules = [
    { num:'01', rule:'NEVER buy above H4', detail:'H4 is the statistical reversal zone. 85%+ of moves reverse here. Smart money sells at H4.' },
    { num:'02', rule:'PP is your compass', detail:'Above PP = bullish bias, buy dips. Below PP = bearish bias, avoid buying.' },
    { num:'03', rule:'First 15 min = Trap', detail:'9:15–9:30 is institutional manipulation time. Wait for real direction at 9:30.' },
    { num:'04', rule:'1:2 R:R Minimum', detail:'Never trade if risk:reward is below 1:2. If risk ₹20, target must be ₹40+.' },
    { num:'05', rule:'Never average options', detail:'Averaging down in options = suicide. Theta decay kills you. Take small loss, move on.' },
  ];

  let html = '';
  rules.forEach(r => {
    html += `<div style="display:flex;gap:12px;padding:10px 0;border-bottom:1px solid var(--border)">
      <div style="font-family:'Orbitron',sans-serif;font-size:20px;font-weight:900;color:var(--gold);flex-shrink:0">${r.num}</div>
      <div>
        <div style="font-size:13px;font-weight:700;margin-bottom:2px">${r.rule}</div>
        <div style="font-size:11px;color:var(--dim);font-family:'Share Tech Mono',monospace;line-height:1.6">${r.detail}</div>
      </div>
    </div>`;
  });
  document.getElementById('goldenRules').innerHTML = html;

  const indicators = [
    { name:'RSI', full:'Relative Strength Index', sig:'<30=Oversold(Buy) | >70=Overbought(Sell) | 50=Neutral', color:'var(--accent)' },
    { name:'MACD', full:'Moving Avg Convergence Divergence', sig:'MACD > Signal = Bull | MACD < Signal = Bear | Zero cross = Strong signal', color:'var(--green)' },
    { name:'ADX', full:'Average Directional Index', sig:'<20=No trend | 20-40=Trend | >40=Strong trend | >60=Extreme', color:'var(--gold)' },
    { name:'AO', full:'Awesome Oscillator', sig:'Green bars = Bull momentum | Red bars = Bear | Crosses zero = Signal', color:'#88ff00' },
    { name:'BB', full:'Bollinger Bands', sig:'Near upper band = Overbought | Near lower = Oversold | Squeeze = Breakout coming', color:'#ff8c42' },
    { name:'KST', full:'Know Sure Thing', sig:'KST > Signal line = Bull | KST < Signal = Bear | Crossover = Strong signal', color:'#ff3e6c' },
    { name:'VWAP', full:'Volume Weighted Avg Price', sig:'Price > VWAP = Bullish | Price < VWAP = Bearish | Used by institutions', color:'var(--accent)' },
  ];

  let indHtml = '';
  indicators.forEach(i => {
    indHtml += `<div style="padding:10px 0;border-bottom:1px solid var(--border)">
      <div style="display:flex;align-items:center;gap:8px;margin-bottom:4px">
        <span style="background:${i.color}22;color:${i.color};padding:2px 8px;border-radius:4px;font-family:'Share Tech Mono',monospace;font-size:11px;font-weight:700">${i.name}</span>
        <span style="font-size:11px;color:var(--dim)">${i.full}</span>
      </div>
      <div style="font-size:11px;color:var(--text);font-family:'Share Tech Mono',monospace;line-height:1.6">${i.sig}</div>
    </div>`;
  });
  document.getElementById('indicatorGuide').innerHTML = indHtml;

  const psychRulesList = [
    { icon:'😱', title:'FEAR = BUY SIGNAL', desc:'When Twitter/Telegram groups are panicking and saying "market will crash" → that\'s the bottom. Smart money buys when retail is selling in panic.' },
    { icon:'🤑', title:'GREED = SELL SIGNAL', desc:'When everyone is posting profits and saying "easy money" → top is near. Smart money distributes when retail is rushing to buy.' },
    { icon:'🐂', title:'BULL TRAP', desc:'Price breaks above resistance with big green candle → retail buys → then immediately reverses down. Always wait for retest.' },
    { icon:'🐻', title:'BEAR TRAP', desc:'Price breaks below support → retail shorts → then immediately reverses up. Stop hunt by institutions before real move.' },
    { icon:'⏳', title:'TIME DECAY (THETA)', desc:'Options lose value every minute you hold. A PE bought at ₹300 can become ₹100 in 2 days even if market doesn\'t move. Buy close to expiry = gamble.' },
  ];

  let psychHtml = '';
  psychRulesList.forEach(r => {
    psychHtml += `<div style="padding:10px 0;border-bottom:1px solid var(--border)">
      <div style="display:flex;align-items:center;gap:8px;margin-bottom:4px">
        <span style="font-size:20px">${r.icon}</span>
        <span style="font-size:12px;font-weight:700;color:var(--accent)">${r.title}</span>
      </div>
      <div style="font-size:11px;color:var(--dim);font-family:'Share Tech Mono',monospace;line-height:1.6">${r.desc}</div>
    </div>`;
  });
  document.getElementById('psychRules').innerHTML = psychHtml;
}

async function askLearnAI() {
  const q = document.getElementById('learnQ').value.trim();
  if(!q) { alert('Please enter a question'); return; }

  document.getElementById('learnLoading').classList.add('show');
  document.getElementById('learnAnswer').style.display = 'none';

  try {
    const res = await fetch('https://api.anthropic.com/v1/messages', {
      method:'POST',
      headers:{'Content-Type':'application/json'},
      body: JSON.stringify({
        model:'claude-sonnet-4-20250514',
        max_tokens:1000,
        messages:[{
          role:'user',
          content:`You are a friendly Indian stock market teacher specializing in options trading (BankNifty, Nifty). Answer this question in simple English with practical examples in Indian market context. Use ₹ for prices. Keep it educational, practical and easy to understand for a beginner.\n\nQuestion: ${q}`
        }]
      })
    });
    const data = await res.json();
    const text = data.content?.map(b=>b.text||'').join('') || 'Could not get answer';
    document.getElementById('learnAnswer').textContent = text;
    document.getElementById('learnAnswer').style.display = 'block';
  } catch(e) {
    document.getElementById('learnAnswer').textContent = '⚠️ Could not connect to AI. Please try again.';
    document.getElementById('learnAnswer').style.display = 'block';
  }
  document.getElementById('learnLoading').classList.remove('show');
}

// ═══════════════════════════════════════════
// INIT
// ═══════════════════════════════════════════
document.addEventListener('DOMContentLoaded', () => {
  setupDragDrop();
  // Load saved zerodha creds
  const savedKey = localStorage.getItem('z_api_key');
  if(savedKey) document.getElementById('zApiKey').value = savedKey;
  const savedToken = localStorage.getItem('z_access_token');
  if(savedToken) document.getElementById('zAccessToken').value = savedToken;
  // Load paper settings
  const ps = localStorage.getItem('paper_settings');
  if(ps) {
    const p = JSON.parse(ps);
    if(p.cap) document.getElementById('maxCapital').value = p.cap;
    if(p.loss) document.getElementById('maxLoss').value = p.loss;
    if(p.tgt) document.getElementById('targetPct').value = p.tgt;
  }
});
</script>
</body>
</html>
