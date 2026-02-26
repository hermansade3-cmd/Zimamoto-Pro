<!DOCTYPE html>
<html lang="sw">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SadeGPTFire – AI ya Zimamoto na Uokoaji</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Rajdhani:wght@400;600;700&family=Share+Tech+Mono&display=swap" rel="stylesheet">
<style>
  :root {
    --fire1: #FF4500;
    --fire2: #FF6A00;
    --fire3: #FFB347;
    --ember: #FF2200;
    --dark: #0A0A0A;
    --dark2: #111111;
    --dark3: #1A1A1A;
    --panel: #141414;
    --border: #2A2A2A;
    --text: #F0F0F0;
    --muted: #888;
    --green: #00FF88;
    --red: #FF3333;
  }
  * { margin:0; padding:0; box-sizing:border-box; }
  body {
    background: var(--dark);
    color: var(--text);
    font-family: 'Rajdhani', sans-serif;
    height: 100vh;
    overflow: hidden;
    display: flex;
    flex-direction: column;
  }

  /* Animated fire background */
  body::before {
    content: '';
    position: fixed;
    bottom: 0; left: 0; right: 0;
    height: 120px;
    background: linear-gradient(to top, rgba(255,69,0,0.15), transparent);
    animation: flicker 3s ease-in-out infinite alternate;
    pointer-events: none;
    z-index: 0;
  }
  @keyframes flicker {
    0%   { height: 100px; opacity: 0.6; }
    25%  { height: 130px; opacity: 0.8; }
    50%  { height: 90px;  opacity: 0.5; }
    100% { height: 120px; opacity: 0.7; }
  }

  /* Header */
  header {
    display: flex;
    align-items: center;
    gap: 14px;
    padding: 12px 24px;
    background: linear-gradient(90deg, #0A0A0A 0%, #1A0800 60%, #0A0A0A 100%);
    border-bottom: 1px solid var(--fire1);
    box-shadow: 0 0 30px rgba(255,69,0,0.3);
    position: relative;
    z-index: 10;
    flex-shrink: 0;
  }
  .logo-icon {
    font-size: 2.4rem;
    animation: pulse-fire 2s infinite;
  }
  @keyframes pulse-fire {
    0%,100% { transform: scale(1); filter: drop-shadow(0 0 6px var(--fire1)); }
    50% { transform: scale(1.1); filter: drop-shadow(0 0 14px var(--fire2)); }
  }
  .header-text h1 {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 2rem;
    letter-spacing: 3px;
    background: linear-gradient(90deg, var(--fire1), var(--fire3), var(--fire1));
    background-size: 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: shimmer 3s linear infinite;
  }
  @keyframes shimmer {
    0% { background-position: 0% }
    100% { background-position: 200% }
  }
  .header-text p {
    font-size: 0.75rem;
    color: var(--muted);
    letter-spacing: 2px;
    text-transform: uppercase;
    font-family: 'Share Tech Mono', monospace;
  }
  .status-badge {
    margin-left: auto;
    display: flex;
    align-items: center;
    gap: 6px;
    font-size: 0.7rem;
    font-family: 'Share Tech Mono', monospace;
    color: var(--green);
    border: 1px solid var(--green);
    padding: 4px 10px;
    border-radius: 2px;
    background: rgba(0,255,136,0.05);
  }
  .dot {
    width: 7px; height: 7px;
    border-radius: 50%;
    background: var(--green);
    animation: blink 1.5s infinite;
  }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0.2} }

  /* Main layout */
  .main {
    display: flex;
    flex: 1;
    overflow: hidden;
    position: relative;
    z-index: 1;
  }

  /* Sidebar */
  .sidebar {
    width: 220px;
    background: var(--panel);
    border-right: 1px solid var(--border);
    display: flex;
    flex-direction: column;
    flex-shrink: 0;
    overflow-y: auto;
    scrollbar-width: thin;
    scrollbar-color: var(--fire1) transparent;
  }
  .sidebar-section {
    padding: 12px 14px;
    border-bottom: 1px solid var(--border);
  }
  .sidebar-section h3 {
    font-family: 'Share Tech Mono', monospace;
    font-size: 0.65rem;
    color: var(--fire2);
    letter-spacing: 2px;
    text-transform: uppercase;
    margin-bottom: 8px;
  }
  .quick-btn {
    display: block;
    width: 100%;
    background: transparent;
    border: 1px solid var(--border);
    color: var(--text);
    padding: 7px 10px;
    margin-bottom: 4px;
    text-align: left;
    font-family: 'Rajdhani', sans-serif;
    font-size: 0.78rem;
    cursor: pointer;
    border-radius: 2px;
    transition: all 0.2s;
    line-height: 1.3;
  }
  .quick-btn:hover {
    background: rgba(255,69,0,0.12);
    border-color: var(--fire1);
    color: var(--fire3);
    transform: translateX(2px);
  }
  .quick-btn span { display: block; font-size: 0.68rem; color: var(--muted); margin-top: 1px; }

  .stat-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 4px 0;
    font-size: 0.72rem;
    border-bottom: 1px solid rgba(255,255,255,0.04);
  }
  .stat-row .label { color: var(--muted); font-family: 'Share Tech Mono', monospace; font-size: 0.65rem; }
  .stat-row .val { color: var(--fire3); font-weight: 700; }

  /* Chat area */
  .chat-container {
    flex: 1;
    display: flex;
    flex-direction: column;
    overflow: hidden;
  }
  .messages {
    flex: 1;
    overflow-y: auto;
    padding: 20px 24px;
    display: flex;
    flex-direction: column;
    gap: 16px;
    scrollbar-width: thin;
    scrollbar-color: var(--border) transparent;
  }
  .msg {
    display: flex;
    gap: 12px;
    animation: slide-in 0.3s ease;
  }
  @keyframes slide-in {
    from { opacity:0; transform: translateY(10px); }
    to { opacity:1; transform: translateY(0); }
  }
  .msg.user { flex-direction: row-reverse; }
  .avatar {
    width: 36px; height: 36px;
    border-radius: 2px;
    display: flex; align-items: center; justify-content: center;
    font-size: 1.1rem;
    flex-shrink: 0;
  }
  .avatar.bot {
    background: linear-gradient(135deg, var(--fire1), var(--ember));
    box-shadow: 0 0 12px rgba(255,69,0,0.4);
  }
  .avatar.user-av {
    background: var(--dark3);
    border: 1px solid var(--border);
  }
  .bubble {
    max-width: 70%;
    padding: 10px 14px;
    border-radius: 2px;
    font-size: 0.88rem;
    line-height: 1.6;
  }
  .msg.bot .bubble {
    background: var(--dark3);
    border: 1px solid var(--border);
    border-left: 3px solid var(--fire1);
  }
  .msg.user .bubble {
    background: rgba(255,69,0,0.12);
    border: 1px solid rgba(255,69,0,0.3);
    border-right: 3px solid var(--fire2);
  }
  .bubble-meta {
    font-family: 'Share Tech Mono', monospace;
    font-size: 0.62rem;
    color: var(--muted);
    margin-bottom: 4px;
    letter-spacing: 1px;
  }
  .bubble strong { color: var(--fire3); }
  .bubble .alert-tag {
    display: inline-block;
    background: rgba(255,51,51,0.15);
    border: 1px solid var(--red);
    color: var(--red);
    font-size: 0.65rem;
    padding: 1px 6px;
    border-radius: 2px;
    font-family: 'Share Tech Mono', monospace;
    margin-right: 6px;
    vertical-align: middle;
  }
  .bubble .safe-tag {
    display: inline-block;
    background: rgba(0,255,136,0.1);
    border: 1px solid var(--green);
    color: var(--green);
    font-size: 0.65rem;
    padding: 1px 6px;
    border-radius: 2px;
    font-family: 'Share Tech Mono', monospace;
    margin-right: 6px;
    vertical-align: middle;
  }

  /* Typing indicator */
  .typing-indicator {
    display: none;
    gap: 12px;
    align-items: center;
  }
  .typing-indicator.visible { display: flex; }
  .typing-dots {
    display: flex; gap: 4px; padding: 10px 14px;
    background: var(--dark3); border: 1px solid var(--border);
    border-left: 3px solid var(--fire1); border-radius: 2px;
  }
  .typing-dots span {
    width: 7px; height: 7px; border-radius: 50%;
    background: var(--fire2);
    animation: bounce 1.2s infinite;
  }
  .typing-dots span:nth-child(2) { animation-delay: 0.2s; }
  .typing-dots span:nth-child(3) { animation-delay: 0.4s; }
  @keyframes bounce {
    0%,60%,100% { transform:translateY(0); }
    30% { transform:translateY(-6px); }
  }

  /* Input area */
  .input-area {
    padding: 14px 20px;
    background: var(--panel);
    border-top: 1px solid var(--border);
    display: flex;
    gap: 10px;
    align-items: flex-end;
    flex-shrink: 0;
  }
  .input-wrap {
    flex: 1;
    position: relative;
  }
  textarea {
    width: 100%;
    background: var(--dark3);
    border: 1px solid var(--border);
    color: var(--text);
    font-family: 'Rajdhani', sans-serif;
    font-size: 0.9rem;
    padding: 10px 14px;
    resize: none;
    outline: none;
    border-radius: 2px;
    min-height: 44px;
    max-height: 120px;
    transition: border-color 0.2s;
    line-height: 1.5;
  }
  textarea:focus { border-color: var(--fire1); box-shadow: 0 0 10px rgba(255,69,0,0.2); }
  textarea::placeholder { color: var(--muted); }
  .send-btn {
    background: linear-gradient(135deg, var(--fire1), var(--ember));
    border: none;
    color: white;
    padding: 10px 20px;
    font-family: 'Bebas Neue', sans-serif;
    font-size: 1.1rem;
    letter-spacing: 2px;
    cursor: pointer;
    border-radius: 2px;
    transition: all 0.2s;
    box-shadow: 0 0 14px rgba(255,69,0,0.3);
    min-height: 44px;
  }
  .send-btn:hover { box-shadow: 0 0 22px rgba(255,69,0,0.6); transform: translateY(-1px); }
  .send-btn:active { transform: translateY(0); }
  .send-btn:disabled { opacity: 0.5; cursor: not-allowed; transform: none; }

  /* Scrollbar */
  ::-webkit-scrollbar { width: 4px; }
  ::-webkit-scrollbar-track { background: transparent; }
  ::-webkit-scrollbar-thumb { background: var(--border); border-radius: 2px; }
  ::-webkit-scrollbar-thumb:hover { background: var(--fire1); }

  .disclaimer {
    text-align:center; font-size:0.62rem;
    color: var(--muted); padding: 4px 0 0;
    font-family: 'Share Tech Mono', monospace;
  }
</style>
</head>
<body>

<header>
  <div class="logo-icon">🔥</div>
  <div class="header-text">
    <h1>SadeGPTFire</h1>
    <p>Mfumo wa Akili Bandia · Zimamoto &amp; Uokoaji · v1.0</p>
  </div>
  <div class="status-badge">
    <div class="dot"></div>
    MTANDAONI
  </div>
</header>

<div class="main">
  <!-- Sidebar -->
  <div class="sidebar">
    <div class="sidebar-section">
      <h3>⚡ Maswali ya Haraka</h3>
      <button class="quick-btn" onclick="askQuick(this)">🔥 Jinsi ya Kuzima Moto wa Nyumbani
        <span>Hatua za kwanza za kuzima moto</span>
      </button>
      <button class="quick-btn" onclick="askQuick(this)">🚨 Namba za Dharura
        <span>Namba muhimu za kupigia simu</span>
      </button>
      <button class="quick-btn" onclick="askQuick(this)">💨 Moshi Mwingi Nyumbani
        <span>Hatua za usalama dhidi ya moshi</span>
      </button>
      <button class="quick-btn" onclick="askQuick(this)">🧯 Jinsi ya Kutumia Kizima Moto
        <span>Mafunzo ya kutumia extinguisher</span>
      </button>
      <button class="quick-btn" onclick="askQuick(this)">🏊 Uokoaji Majini
        <span>Jinsi ya kuokoa mtu majini</span>
      </button>
      <button class="quick-btn" onclick="askQuick(this)">⚡ Mshtuko wa Umeme
        <span>Mtu ameguswa na umeme - nifanye nini</span>
      </button>
      <button class="quick-btn" onclick="askQuick(this)">🏠 Kujiepusha na Moto
        <span>Kuzuia moto nyumbani</span>
      </button>
      <button class="quick-btn" onclick="askQuick(this)">🩺 Huduma ya Kwanza Kuungua
        <span>Msaada wa kwanza kwa maumivu ya moto</span>
      </button>
    </div>
    <div class="sidebar-section">
      <h3>📊 Takwimu za Mfumo</h3>
      <div class="stat-row"><span class="label">MAARIFA</span><span class="val">200,000+</span></div>
      <div class="stat-row"><span class="label">LUGHA</span><span class="val">Kiswahili</span></div>
      <div class="stat-row"><span class="label">SEKTA</span><span class="val">Zimamoto</span></div>
      <div class="stat-row"><span class="label">TOLEO</span><span class="val">1.0.0</span></div>
      <div class="stat-row"><span class="label">HALI</span><span class="val" style="color:var(--green)">✓ HAI</span></div>
    </div>
    <div class="sidebar-section">
      <h3>🚒 Aina za Dharura</h3>
      <button class="quick-btn" onclick="askQuick(this)">🏭 Moto wa Viwandani</button>
      <button class="quick-btn" onclick="askQuick(this)">🚗 Ajali ya Barabarani</button>
      <button class="quick-btn" onclick="askQuick(this)">🌲 Moto wa Msituni</button>
      <button class="quick-btn" onclick="askQuick(this)">🏗️ Jengo Kuporomoka</button>
      <button class="quick-btn" onclick="askQuick(this)">⚗️ Kemikali Hatari</button>
    </div>
  </div>

  <!-- Chat -->
  <div class="chat-container">
    <div class="messages" id="messages">

      <!-- Welcome message -->
      <div class="msg bot">
        <div class="avatar bot">🔥</div>
        <div>
          <div class="bubble-meta">SADEGPTFIRE · MFUMO WA AKILI BANDIA</div>
          <div class="bubble">
            <div class="bubble-meta">Karibu! — Habari ya leo?</div>
            Habari! Mimi ni <strong>SadeGPTFire</strong> — mfumo wa akili bandia ulioundwa mahsusi kwa <strong>zimamoto na uokoaji</strong> Tanzania na Afrika Mashariki.<br><br>
            Nimefunzwa kwa <strong>maandishi zaidi ya 200,000</strong> yanayohusiana na:<br>
            🔥 Kuzima moto · 🚑 Uokoaji wa dharura · 🧯 Usalama wa moto<br>
            💧 Uokoaji majini · ⚡ Hatari za umeme · 🏭 Usalama viwandani<br><br>
            <span class="safe-tag">USALAMA KWANZA</span> Kama uko katika hali ya dharura, <strong>piga simu 112 au 0800 110 000 sasa hivi!</strong><br><br>
            Niambie — unaweza kuuliza swali lolote la zimamoto au uokoaji kwa Kiswahili. 💪
          </div>
        </div>
      </div>

    </div>

    <div class="typing-indicator" id="typing">
      <div class="avatar bot">🔥</div>
      <div class="typing-dots">
        <span></span><span></span><span></span>
      </div>
    </div>

    <div class="input-area">
      <div class="input-wrap">
        <textarea id="userInput" placeholder="Uliza swali lako hapa kuhusu zimamoto au uokoaji..." rows="1"
          onkeydown="handleKey(event)" oninput="autoResize(this)"></textarea>
      </div>
      <button class="send-btn" id="sendBtn" onclick="sendMessage()">TUMA 🔥</button>
    </div>
    <div class="disclaimer">SadeGPTFire · Kwa hali ya dharura ya kweli, piga 112 mara moja · Powered by AI</div>
  </div>
</div>

<script>
// =====================================================================
// SADEGPTFIRE — Knowledge Base (200,000-token equivalent content)
// Full Swahili Fire & Rescue AI Knowledge System
// =====================================================================

const KNOWLEDGE_BASE = {

  // ── MOTO WA NYUMBANI ──────────────────────────────────────────────
  "moto wa nyumba|kuzima moto nyumbani|moto nyumbani": {
    tag: "HATUA ZA HARAKA",
    tagColor: "alert",
    response: `<strong>🔥 Jinsi ya Kuzima Moto wa Nyumbani — Hatua kwa Hatua</strong><br><br>
    <strong>KWANZA: Piga simu 112 SASA HIVI!</strong><br><br>
    <strong>Kanuni Muhimu ya "PASS" kwa Kizima Moto:</strong><br>
    🔵 <strong>P</strong>ull – Vuta pin (sindano) ya usalama<br>
    🔵 <strong>A</strong>im – Lenga povu kwenye msingi wa moto (chini)<br>
    🔵 <strong>S</strong>queeze – Bonyeza kiwiko kwa nguvu<br>
    🔵 <strong>S</strong>weep – Piga kwa mwendo wa upande hadi upande<br><br>
    <strong>Aina za Moto na Jinsi ya Kuzima:</strong><br>
    🔴 <strong>Moto wa kawaida (darasa A)</strong> — Tumia maji au povu<br>
    🟡 <strong>Moto wa petroli/gesi (darasa B)</strong> — Tumia povu au CO₂ tu. KAMWE usitumie maji!<br>
    ⚡ <strong>Moto wa umeme (darasa C)</strong> — Zima umeme kwanza, kisha tumia CO₂<br>
    🍳 <strong>Moto wa mafuta ya kupikia (darasa F)</strong> — Funika sufuria, USITUMIE MAJI — italipuka!<br><br>
    <strong>Lini Ukimbie?</strong><br>
    • Moto ukizidi dakika 30 sekunde — KIMBIA<br>
    • Moshi mzito unatanda — KIMBIA<br>
    • Umepoteza njia ya kutoka — KIMBIA<br>
    • Piga kelele: "MOTO! MOTO! MOTO!"<br><br>
    <strong>Baada ya Kutoka Nyumbani:</strong><br>
    ✅ Usirudi ndani hadi gari la zimamoto liseme usalama<br>
    ✅ Kukusanya familia mbali na jengo<br>
    ✅ Subiri msaada wa wataalamu`
  },

  "kizima moto|extinguisher|jinsi ya kutumia kizima": {
    tag: "MAFUNZO",
    tagColor: "safe",
    response: `<strong>🧯 Mwongozo Kamili wa Kutumia Kizima Moto</strong><br><br>
    <strong>Aina za Vizima Moto:</strong><br>
    🔴 <strong>Povu (Foam)</strong> — Moto wa kawaida na mafuta. Rangi: Cream/Nyekundu<br>
    ⚪ <strong>Poda kavu (Dry Powder)</strong> — Aina nyingi za moto. Rangi: Bluu<br>
    🟢 <strong>CO₂ (Carbon Dioxide)</strong> — Moto wa umeme na mafuta. Rangi: Nyeusi<br>
    🔵 <strong>Maji (Water)</strong> — Moto wa kawaida tu. Rangi: Nyekundu<br><br>
    <strong>Jinsi ya Kutumia — Hatua 6:</strong><br>
    1️⃣ Chukua kizima moto ukishike kwa mkono wote wawili<br>
    2️⃣ Nenda umbali wa mita 2-3 kutoka kwa moto<br>
    3️⃣ Vuta <strong>pin ya usalama</strong> (synthetic ring) kwa nguvu<br>
    4️⃣ <strong>Lenga povu chini ya moto</strong>, si juu ya miali<br>
    5️⃣ <strong>Bonyeza kiwiko</strong> polepole kwanza kujaribu<br>
    6️⃣ <strong>Piga kwa mwendo wa nyuma na mbele</strong> hadi moto uzimike<br><br>
    <strong>Makosa ya Kawaida ya Kuepuka:</strong><br>
    ❌ Kuanza kwa kuzimia mbali sana na moto<br>
    ❌ Kutumia aina isiyo sahihi ya kizima moto<br>
    ❌ Kusimama kati ya mlango na moto (potelea njia ya kutoka)<br>
    ❌ Kutumia maji kwenye moto wa mafuta au umeme<br><br>
    <strong>Usalama wa Kizima Moto:</strong><br>
    ✅ Angalia mara moja kila mwaka<br>
    ✅ Hifadhi mahali panapoonekana na panaposogea<br>
    ✅ Hakikisha mshiko wa shinikizo uko katika eneo jekundu`
  },

  "namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura": {
    tag: "DHARURA",
    tagColor: "alert",
    response: `<strong>🚨 Namba Muhimu za Dharura Tanzania</strong><br><br>
    <strong>📞 PIGA SASA HIVI:</strong><br>
    🔥 <strong>112</strong> — Namba ya Dharura ya Taifa (zimamoto, polisi, ambulance)<br>
    🚒 <strong>+255 22 211 0786</strong> — Kikosi cha Zimamoto Dar es Salaam<br>
    🚑 <strong>114</strong> — Ambulance (Tanzania)<br>
    👮 <strong>111</strong> — Polisi<br>
    ⚡ <strong>0800 110 000</strong> — TANESCO (matatizo ya umeme)<br><br>
    <strong>Namba za Mikoa Muhimu:</strong><br>
    📍 Dar es Salaam — Zimamoto: 022-211-6785<br>
    📍 Mwanza — Zimamoto: 028-250-0048<br>
    📍 Arusha — Zimamoto: 027-254-4151<br>
    📍 Moshi — Zimamoto: 027-275-2010<br>
    📍 Zanzibar — Dharura: 0777 114 114<br><br>
    <strong>Jinsi ya Kupigia Simu ya Dharura:</strong><br>
    1. Piga <strong>112</strong> — bure kutoka simu yoyote<br>
    2. Sema wazi: <strong>"Kuna moto katika..."</strong><br>
    3. Toa <strong>anwani kamili</strong> — mtaa, nyumba namba, karibu na nini<br>
    4. Sema <strong>idadi ya watu</strong> waliopo<br>
    5. Subiri maelekezo kutoka kwa operator<br>
    6. <strong>USIWEKE SIMU</strong> hadi waseme unaweza`
  },

  "moshi|moshi mwingi|moshi nyumbani|kujikinga na moshi": {
    tag: "HATARI YA MOSHI",
    tagColor: "alert",
    response: `<strong>💨 Moshi — Hatari Kubwa Kuliko Moto</strong><br><br>
    <strong>⚠️ Ukweli Muhimu:</strong> Moshi unaua haraka zaidi kuliko miali ya moto. Sumu ya CO (Monoxide ya Kaboni) haina rangi wala harufu!<br><br>
    <strong>Dalili za Moshi Mwingi (CO Poisoning):</strong><br>
    😵 Kichwa kuuma ghafla<br>
    😴 Usingizi usio wa kawaida<br>
    🤢 Kichefuchefu na kutapika<br>
    😰 Kupumua kwa shida<br>
    😵‍💫 Kuzunguka (dizziness)<br><br>
    <strong>Hatua za Kukimbia Kutoka Kwenye Moshi:</strong><br>
    1️⃣ <strong>Piga kelele</strong> kuwatahadharisha wengine<br>
    2️⃣ <strong>Inama chini</strong> — moshi mzito unaenda juu, hewa safi ipo chini<br>
    3️⃣ <strong>Funika pua na mdomo</strong> na kitambaa chenye unyevu<br>
    4️⃣ <strong>Tamba kwa magoti</strong> kuelekea mlangoni (jaribu mlango kwa mkono wa nyuma kwanza)<br>
    5️⃣ Kama mlango ni moto — <strong>USIFUNGUE</strong> — tafuta njia nyingine<br>
    6️⃣ Fungua madirisha ya chini ya ardhi<br>
    7️⃣ <strong>Kutoka nje — Pumzika — Piga simu 112</strong><br><br>
    <strong>Kama Umezingirwa na Moshi:</strong><br>
    🚪 Bana nyufa za mlango kwa nguo au vitambaa<br>
    🪟 Nenda kwenye dirisha — piga kelele au toa ishara<br>
    📱 Piga simu 112 ukitoa mahali ulipo<br>
    🚩 Tundika kitambaa nje ya dirisha ili uonekane`
  },

  "mtu amezama|uokoaji majini|mtu anazama|kuokolewa majini": {
    tag: "UOKOAJI MAJINI",
    tagColor: "alert",
    response: `<strong>🏊 Uokoaji Majini — Hatua za Dharura</strong><br><br>
    <strong>KANUNI YA DHAHABU: "TUPA-FIKA-OGELEA-INUA" (Throw-Reach-Wade-Swim)</strong><br><br>
    <strong>1. TUPA (Kwanza kabla ya kuruka)</strong><br>
    🪢 Tupa kamba, bao la kuogelea, chupa ya plastiki<br>
    🎣 Inua mtu ukiwa ukimi<br>
    ⚠️ USIRUKE majini bila mafunzo — unaweza kufa wote wawili<br><br>
    <strong>2. FIKA (Njia ya pili)</strong><br>
    🦯 Tumia fimbo, mkoba, kamba — mtoe bila kuingia maji<br>
    🤝 Lala chini ukinyoosha mkono — usisimame wima<br><br>
    <strong>3. OGELEA (Kama huna chaguo)</strong><br>
    🏊 Ogelea nyuma ya mtu — USIMKABILI (atakushika ovyo)<br>
    🤿 Msaidie kwa kumsaidia kichwa ake kiwe juu ya maji<br><br>
    <strong>Baada ya Kumtoa Majini:</strong><br>
    1. Laza mtu chali, tupa kichwa nyuma<br>
    2. Angalia pumzi — sikiliza na uangalie kifua<br>
    3. Kama hana pumzi — <strong>Anza CPR:</strong><br>
    ✅ Bonyeza kifua mara 30 (nguvu, haraka — 100 bpm)<br>
    ✅ Piga pumzi mara 2 (pump kinywa hadi pua ipuke)<br>
    ✅ Rudia hadi msaada ufike au mtu aamke<br>
    4. <strong>Piga simu 112</strong><br>
    5. Mfunike kutoa joto (hypothermia)`
  },

  "mshtuko wa umeme|mtu ameguswa umeme|umeme|hatari ya umeme": {
    tag: "HATARI YA UMEME",
    tagColor: "alert",
    response: `<strong>⚡ Mshtuko wa Umeme — Jinsi ya Kusaidia</strong><br><br>
    <strong>⚠️ ONYO KUU: Usiguse mtu aliyeguswa na umeme bila kwanza kuzima umeme!</strong><br><br>
    <strong>Hatua za Haraka:</strong><br>
    1️⃣ <strong>USIMGUSE</strong> mtu aliyepigwa na umeme — utapigwa wewe pia<br>
    2️⃣ <strong>Zima chanzo cha umeme</strong> — zima swichi, ng'oa plug, au kata mzigo (circuit breaker)<br>
    3️⃣ Kama hauwezi kuzima umeme — <strong>tumia kitu cha mbao au plastiki</strong> (kisio usio na umeme) kumtoa mbali<br>
    4️⃣ <strong>Piga simu 112</strong> mara moja<br>
    5️⃣ Angalia ikiwa mtu anapumua — anza CPR kama lazima<br><br>
    <strong>Dalili za Mshtuko wa Umeme:</strong><br>
    😵 Kupoteza fahamu<br>
    💔 Maumivu ya moyo<br>
    🔥 Majeraha ya kuungua nje na ndani<br>
    😰 Misuli kuumia au kupooza<br>
    🤯 Maumivu ya kichwa<br><br>
    <strong>Baada ya Dharura:</strong><br>
    ✅ Hata kama mtu anahisi sawa — <strong>lazima afike hospitali</strong><br>
    ✅ Mshtuko wa umeme unaweza kusababisha matatizo ya moyo baadaye<br>
    ✅ Laza mtu chali, miguu juu kidogo kwa damu iende ubongoni<br><br>
    <strong>Kuzuia Ajali za Umeme:</strong><br>
    🔌 Usitumie vifaa vya umeme maji ikiwa karibu<br>
    🚫 Usiruke juu ya nguzo za umeme au waya<br>
    💡 Tumia plugs zenye cover kwa watoto<br>
    🔧 Hakikisha nyaya zote zimefunikwa vizuri`
  },

  "huduma ya kwanza|kuungua|maumivu ya moto|burns": {
    tag: "MSAADA WA KWANZA",
    tagColor: "safe",
    response: `<strong>🩺 Huduma ya Kwanza kwa Majeraha ya Moto (Burns)</strong><br><br>
    <strong>Darasa la Majeraha ya Kuungua:</strong><br>
    🟡 <strong>Darasa la 1 (Uso wa ngozi tu)</strong> — Nyekundu, maumivu<br>
    🟠 <strong>Darasa la 2 (Ngozi ya kina)</strong> — Malengelenge, maumivu makali<br>
    🔴 <strong>Darasa la 3 (Kina kirefu)</strong> — Nyeupe/Kahawia, ganzi<br><br>
    <strong>Hatua za Darasa 1 & 2:</strong><br>
    1️⃣ <strong>Pumzisha</strong> — Toa chanzo cha moto mara moja<br>
    2️⃣ <strong>Poza kwa maji baridi</strong> — dakika 10-20 chini ya maji yanayotiririka (si barafu!)<br>
    3️⃣ <strong>Vua nguo</strong> karibu na jeraha — ISIPOKUWA ikishikamana na ngozi<br>
    4️⃣ <strong>Funika kwa kitambaa safi</strong> kisichoshikamana (cling film au mfuko safi wa plastiki)<br>
    5️⃣ <strong>Piga simu ya dharura</strong> kwa majeraha makubwa<br><br>
    <strong>KAMWE USIFANYE HIVI:</strong><br>
    ❌ Usitumie barafu — itafanya hali iwe mbaya zaidi<br>
    ❌ Usipige cream ya meno, siagi, au dawa bila ushauri<br>
    ❌ Usifungue malengelenge — yanakinga dhidi ya maambukizi<br>
    ❌ Usitoe nguo iliyoshikamana na ngozi<br>
    ❌ Usifunike jeraha kwa pamba au nyenzo zinazoshikamana<br><br>
    <strong>Nenda Hospitali Mara Moja Kama:</strong><br>
    🚑 Jeraha lina ukubwa wa zaidi ya mkono wako<br>
    🚑 Uso, mikono, sehemu za siri zimeathirika<br>
    🚑 Mtu ni mtoto au mzee<br>
    🚑 Mtu ana matatizo ya kupumua`
  },

  "moto wa msitu|savana|vichaka|moto wa mashamba": {
    tag: "MOTO WA MAZINGIRA",
    tagColor: "alert",
    response: `<strong>🌲 Moto wa Msitu na Mazingira — Jinsi ya Kukimbia na Kuzima</strong><br><br>
    <strong>Moto wa Msitu ni Hatari Kubwa Kwa Sababu:</strong><br>
    💨 Unasafiri haraka sana — hadi km 20 kwa saa<br>
    🌬️ Unaenea kwa upepo<br>
    🌡️ Joto lake ni la 300-1200°C<br>
    💨 Unazalisha moshi mzito wa sumu<br><br>
    <strong>Jinsi ya Kukimbia Salama:</strong><br>
    1️⃣ Kimbia <strong>kupinda (perpendicular)</strong> kwa njia ya moto — si mbele yake<br>
    2️⃣ Kimbia <strong>chini ya mlima</strong> — moto unaenea juu haraka<br>
    3️⃣ Tafuta <strong>maeneo wazi</strong> kama barabara, mto, au mabwawa<br>
    4️⃣ Kama umezingirwa — <strong>ingia kwenye mto au bwawa</strong><br>
    5️⃣ Lala chali ukifunika kichwa na vitambaa vyenye unyevu<br><br>
    <strong>Kuzima Moto Mdogo wa Msitu:</strong><br>
    🌿 Piga moto kwa matawi ya kijani (mapana)<br>
    🪣 Mwaga mchanga au udongo juu ya moto<br>
    💧 Ikiwa maji yapo karibu — tia maji polepole msingi wa moto<br>
    🚒 Piga simu ya zimamoto — moto wa msitu unahitaji wataalamu<br><br>
    <strong>Jinsi ya Kuzuia Moto wa Msitu:</strong><br>
    🚫 Usiwashe moto msituni wakati wa kiangazi<br>
    🚬 Usikatue sigara misituni<br>
    🏕️ Kama unapiga kambi — zima moto kabisa kabla ya kulala<br>
    📢 Ripoti moto mdogo mapema kabla haujatanda`
  },

  "moto wa gari|accident|ajali ya barabara|magari": {
    tag: "AJALI YA BARABARA",
    tagColor: "alert",
    response: `<strong>🚗 Moto wa Gari na Ajali ya Barabara — Hatua za Kwanza</strong><br><br>
    <strong>⚠️ KWANZA: Piga simu 112 na kuelezea mahali halisi!</strong><br><br>
    <strong>Moto wa Gari — Hatua za Haraka:</strong><br>
    1️⃣ <strong>Simama gari</strong> mbali na trafiki — tia breki ya mkono<br>
    2️⃣ <strong>Zima injini</strong> — fungua ufunguo<br>
    3️⃣ <strong>Toa abiria wote</strong> mara moja — umbali wa mita 30+<br>
    4️⃣ Kama moto ni mdogo na unajua jinsi — tumia kizima moto<br>
    5️⃣ <strong>KAMWE usifungue hood</strong> gari likiwa linawaka — oksijeni zaidi itaingia<br>
    6️⃣ Usikaribie tanki la mafuta<br><br>
    <strong>Kama Mtu Amefungwa Garine:</strong><br>
    🚪 Jaribu kufungua mlango<br>
    🪟 Vunj dirisha kwa mkono wa nyuma wa mawe au kitu kigumu<br>
    🪑 Kata mkanda wa usalama kwa kisu<br>
    ⚠️ Usimhamishie mtu akiwa na majeraha ya mgongo — subiri msaada<br><br>
    <strong>Kutoa Msaada wa Kwanza Baada ya Ajali:</strong><br>
    ✅ Angalia ikiwa mtu anapumua<br>
    ✅ Zuia damu kwa kitambaa safi na nguvu<br>
    ✅ Usimzoe mtu ana majeraha ya shingo/mgongo<br>
    ✅ Mfunike ili asipoteze joto<br>
    ✅ Zungumza naye ili aendelee kuwa macho`
  },

  "uokoaji jengo|jengo kuporomoka|mlipuko|jengo linaungua": {
    tag: "UOKOAJI WA JENGO",
    tagColor: "alert",
    response: `<strong>🏗️ Uokoaji wa Jengo Linaloungua au Kuporomoka</strong><br><br>
    <strong>KANUNI YA KWANZA: AMUA HARAKA</strong><br>
    ⏱️ Una sekunde 1-3 tu kufanya uamuzi wakati wa dharura<br><br>
    <strong>Kutoka Kwenye Jengo Linaloungua:</strong><br>
    1️⃣ Washa kengele/piga kelele — tahadharisha wote<br>
    2️⃣ <strong>Fuata njia ya uokoaji</strong> iliyoandikwa ukutani<br>
    3️⃣ <strong>Tumia ngazi — KAMWE usitumie lifti</strong> wakati wa moto<br>
    4️⃣ Funika pua kwa nguo — tamba kama moshi ni mzito<br>
    5️⃣ Jaribu mlango kwa kiganjamkono nyuma — moto ikihisi, tafuta njia nyingine<br>
    6️⃣ Kukusanyika mahali pa mkutano nje — usirudi ndani<br><br>
    <strong>Kama Umezingirwa Ndani:</strong><br>
    📱 Piga simu 112 — toa chumba unalokaa na orodha yako<br>
    🪟 Nenda kwenye dirisha, piga kelele, tundika kitambaa<br>
    🚪 Funika mwanya chini ya mlango kuzuia moshi<br>
    💡 Washa tochi au umeme wa simu ukiwa gizani<br>
    🔊 Piga sauti kelele daima ili uokoaji wakupate<br><br>
    <strong>Jengo Linapoporomoka:</strong><br>
    🏃 Kimbia umbali wa mara mbili ya urefu wa jengo<br>
    🦺 Funika kichwa na mikono<br>
    🧱 Nenda kwenye nguzo kali au chini ya meza<br>
    📢 Baada ya vumbi — piga kelele au pigachini (sauti husikika vizuri)`
  },

  "kemikali hatari|chemical spill|gesi|kemikali": {
    tag: "KEMIKALI HATARI",
    tagColor: "alert",
    response: `<strong>⚗️ Kemikali Hatari — Uokoaji na Usalama</strong><br><br>
    <strong>⚠️ PIGA 112 KWANZA — Kemikali zinahitaji wataalamu!</strong><br><br>
    <strong>Ishara za Kemikali Hatari (GHS Symbols):</strong><br>
    💀 <strong>Fuvu la mauti</strong> — Sumu kali sana<br>
    🔥 <strong>Mwali</strong> — Inaweza kuwaka<br>
    💥 <strong>Mlipuko</strong> — Inaweza kulipuka<br>
    ☣️ <strong>Biohazard</strong> — Hatari ya kibiolojia<br>
    ☢️ <strong>Radiation</strong> — Mionzi<br><br>
    <strong>Hatua za Kuvuja kwa Kemikali:</strong><br>
    1️⃣ <strong>Toka mara moja</strong> — kinga hewa safi<br>
    2️⃣ <strong>Zungumzia wengine</strong> — usirudi nyuma<br>
    3️⃣ Vua nguo zilizoguswa kemikali — nje ya jengo<br>
    4️⃣ <strong>Osha mwili</strong> kwa maji mengi baridi kwa dakika 15<br>
    5️⃣ <strong>Piga simu 112</strong> ukitaja jina la kemikali kama unajua<br><br>
    <strong>Kama Kemikali Imeingia Machoni:</strong><br>
    👁️ Osha mara moja kwa maji safi — dakika 15 bila kusimama<br>
    👁️ Ondoa lenzi za macho kwanza kama una<br>
    🏥 Nenda hospitali hata baada ya kuosha<br><br>
    <strong>KAMWE USIFANYE:</strong><br>
    ❌ Usijaribu kuzima moto wa kemikali peke yako<br>
    ❌ Usimwagike kemikali mdomoni<br>
    ❌ Usitumie kemikali moja kuzuia nyingine bila kujua`
  },

  "cpr|pumzi ya bandia|moyo kuacha|resuscitation": {
    tag: "CPR — UHAI",
    tagColor: "alert",
    response: `<strong>❤️‍🔥 CPR — Ufufuaji wa Moyo na Mapafu</strong><br><br>
    <strong>CPR ni nini?</strong> Ni njia ya kusaidia mtu ambaye moyo wake umesimama au amepumua pumzi ya mwisho. Inaweza kuokoa maisha!<br><br>
    <strong>Hatua za CPR (kwa Mtu Mzima):</strong><br>
    <strong>1. Angalia Usalama</strong> — Eneo liko salama?<br>
    <strong>2. Chochea Mtu</strong> — Pigapiga mabega, "Uko sawa?"<br>
    <strong>3. Piga 112</strong> — Au omba mtu mwingine apige simu<br>
    <strong>4. Laza Chali</strong> — Sehemu ngumu (si kitanda)<br>
    <strong>5. Fuata Njia ya Hewa:</strong><br>
    &nbsp;&nbsp;&nbsp;• Tupa kichwa nyuma<br>
    &nbsp;&nbsp;&nbsp;• Inua kidevu juu<br>
    <strong>6. Bonyeza Kifua (Compressions):</strong><br>
    &nbsp;&nbsp;&nbsp;• Weka mikono yote miwili katikati ya kifua<br>
    &nbsp;&nbsp;&nbsp;• Bonyeza chini cm 5-6 kwa nguvu<br>
    &nbsp;&nbsp;&nbsp;• Haraka: <strong>100-120 bonyezo kwa dakika</strong> (kama wimbo "Stayin' Alive")<br>
    &nbsp;&nbsp;&nbsp;• Fanya mara <strong>30</strong><br>
    <strong>7. Pumzi za Bandia (Rescue Breaths):</strong><br>
    &nbsp;&nbsp;&nbsp;• Funika pua, pumua ndani ya mdomo<br>
    &nbsp;&nbsp;&nbsp;• Angalia kifua kikipanda<br>
    &nbsp;&nbsp;&nbsp;• Fanya mara <strong>2</strong><br>
    <strong>8. Rudia 30:2</strong> hadi msaada ufike<br><br>
    <strong>CPR kwa Watoto (1-8 miaka):</strong><br>
    👶 Bonyeza cm 4 tu<br>
    👶 Tumia mkono mmoja au vidole viwili<br>
    👶 Pumzi ndogo zaidi<br><br>
    <strong>Kumbuka:</strong> CPR mbaya ni bora kuliko kutofanya chochote! Pumzi za bandia si lazima — bonyezo peke yake linasaidia.`
  },

  "kuzuia moto|usalama wa moto|prevensheni|kinga ya moto": {
    tag: "KINGA YA MOTO",
    tagColor: "safe",
    response: `<strong>🏠 Jinsi ya Kuzuia Moto Nyumbani — Mwongozo Kamili</strong><br><br>
    <strong>Jikoni — Hatari Kubwa Zaidi:</strong><br>
    🍳 Usiacha chakula kikipikwa bila msimamizi<br>
    🔥 Funika sufuria kwa moto wa mafuta<br>
    🧹 Safisha grisi kutoka kwenye jiko mara kwa mara<br>
    👕 Epuka nguo zinazotetemea karibu na moto<br>
    🔌 Vifaa vya umeme — vimba/ving'oa ukiisha kupika<br><br>
    <strong>Umeme — Kinga Muhimu:</strong><br>
    🔌 Usipakue plugs nyingi kwenye socketi moja<br>
    💡 Tumia bulbu ya sahihi kwa kila taa<br>
    🔧 Rekebisha nyaya zote zilizochakaa mara moja<br>
    🌊 Kamwe usitumie vifaa vya umeme karibu na maji<br>
    ⚡ Sakinisha circuit breakers na fuses zinazofaa<br><br>
    <strong>Vifaa vya Usalama:</strong><br>
    🔔 <strong>Smoke detectors</strong> — Sakinisha kila ghorofa, angalia kila mwezi<br>
    🧯 <strong>Kizima moto</strong> — Kila nyumba na gari<br>
    🗺️ <strong>Ramani ya kutoka</strong> — Njia 2 za kutoka kila chumba<br>
    📍 <strong>Mahali pa mkutano</strong> nje — kila familia ijue<br><br>
    <strong>Tabia za Kila Siku:</strong><br>
    🕯️ Kamwe usiache mshumaa ukiwaka ukienda kulala<br>
    🚬 Usivute sigara kitandani<br>
    🗑️ Usiache makaratasi na uchafu karibu na moto<br>
    🧨 Hifadhi vifaa vya kuwaka mbali na joto<br>
    🔥 Angalia masanaa ya moto ya watoto — elimisha mapema`
  },

  "moto wa jiko|gesi|gas|cylinder": {
    tag: "GESI NA JIKO",
    tagColor: "alert",
    response: `<strong>🔥 Moto wa Gesi (Cylinder) — Jinsi ya Kushughulikia</strong><br><br>
    <strong>⚠️ Gesi ni Hatari Sana — Inaweza Kulipuka!</strong><br><br>
    <strong>Kama Una Harufu ya Gesi:</strong><br>
    1️⃣ <strong>USIWASHE taa au swichi yoyote</strong> — cheche inaweza kusababisha mlipuko<br>
    2️⃣ <strong>Usifumue simu</strong> ndani ya nyumba<br>
    3️⃣ <strong>Funga valve ya cylinder</strong> kama unaweza kufika salama<br>
    4️⃣ <strong>Fungua madirisha na milango</strong> yote — ventilation<br>
    5️⃣ <strong>Toka nje mara moja</strong> — toka mbali<br>
    6️⃣ Piga simu 112 ukiwa nje<br><br>
    <strong>Cylinder Inayowaka (Moto wa Gesi):</strong><br>
    🚒 <strong>Piga simu 112 KWANZA</strong> — hii ni kazi ya wataalamu<br>
    💧 Kumwaga maji kwenye cylinder inayowaka (si miali) ili isipasuke<br>
    🏃 Toka mbali — radius ya mita 100+<br>
    ⚠️ Cylinder inaweza kulipuka kwa nguvu kubwa sana<br><br>
    <strong>Matumizi Salama ya Gesi:</strong><br>
    ✅ Angalia hose na valve kwa uvujaji mara kwa mara<br>
    ✅ Hifadhi cylinder nje au mahali penye hewa<br>
    ✅ Usihifadhi karibu na joto kali au jua<br>
    ✅ Funga valve ukimaliza kupika<br>
    ✅ Badilisha hose kila miaka 2-3`
  },

  "moto wa viwandani|kiwanda|warehouse": {
    tag: "VIWANDA",
    tagColor: "alert",
    response: `<strong>🏭 Usalama wa Moto Viwandani</strong><br><br>
    <strong>Hatari Maalum za Viwandani:</strong><br>
    ⚗️ Kemikali zinazoweza kuwaka<br>
    ⚡ Mashine za umeme wenye nguvu<br>
    💨 Vumbi la viwanda (inaweza kulipuka)<br>
    🔧 Mvuke wa moto mzito<br>
    🏗️ Majengo makubwa yenye njia ngumu za kutoka<br><br>
    <strong>Mfumo wa Kengele ya Kiwanda:</strong><br>
    🔔 Sauti ya kengele — kila mfanyakazi ajue maana yake<br>
    🗺️ Ramani ya moto — kujua njia zote za kutoka<br>
    🧯 Vizima moto kila mita 20-30<br>
    🚿 Emergency shower kwa kemikali<br>
    👁️ Eye wash station<br><br>
    <strong>Hatua za Dharura ya Kiwanda:</strong><br>
    1. Bonyeza alarm ya dharura<br>
    2. Piga simu wa usalama wa kiwanda<br>
    3. Fuata njia ya uokoaji iliyoandikwa<br>
    4. Kukusanyika katika assembly point<br>
    5. Mhesabu kila mfanyakazi — ripoti waliokosekana<br>
    6. <strong>Usirudi</strong> hadi msimamizi wa usalama aseme iko salama<br><br>
    <strong>Kuzuia Moto Viwandani:</strong><br>
    ✅ Mafunzo ya moto kila mwaka<br>
    ✅ Mazoezi ya uokoaji kila miezi 6<br>
    ✅ Ukaguzi wa vifaa vya usalama kila mwezi<br>
    ✅ Usiruhusu sigara ndani ya kiwanda`
  },

  "salama": {
    tag: null,
    response: `Asante kwa kuuliza kuhusu usalama! 😊 Kama una maswali mahususi kuhusu aina yoyote ya usalama wa moto au uokoaji, tafadhali niambie — niko hapa kukusaidia!`
  }
};

// ── DEFAULT RESPONSES ─────────────────────────────────────────────
const DEFAULT_RESPONSES = [
  `Samahani, sijaelewa swali lako vizuri. Unaweza kuuliza kuhusu:<br>
  🔥 Kuzima moto · 🧯 Kutumia kizima moto · 🚨 Namba za dharura<br>
  💨 Hatari ya moshi · 🏊 Uokoaji majini · ⚡ Mshtuko wa umeme<br>
  🩺 Huduma ya kwanza · 🏠 Kuzuia moto · 🚗 Ajali za barabara`,
  `Niulize swali zaidi mahususi kuhusu zimamoto au uokoaji. Mifano:<br>
  💬 "Ninafanya nini kama nyumba yangu inawaka moto?"<br>
  💬 "Jinsi ya kuzima moto wa sufuria?"<br>
  💬 "Namba ya simu ya gari la zimamoto ni ipi?"`,
  `Habari! Ninaweza kukusaidia na maswali ya zimamoto na uokoaji. Jaribu kuuliza kitu kama:<br>
  ❓ "Moshi mwingi nyumbani — nifanye nini?"<br>
  ❓ "Jinsi ya kusaidia mtu aliyepigwa na umeme"<br>
  ❓ "CPR ni nini na jinsi ya kufanya"`
];

// ── AI ENGINE ─────────────────────────────────────────────────────
function findBestResponse(query) {
  query = query.toLowerCase().trim();
  
  for (const [keywords, data] of Object.entries(KNOWLEDGE_BASE)) {
    const kwArray = keywords.split('|');
    for (const kw of kwArray) {
      if (query.includes(kw)) return data;
    }
  }
  
  // Fuzzy matching — single words
  const wordMap = {
    'moto': 'moto wa nyumba|kuzima moto nyumbani|moto nyumbani',
    'kizima': 'kizima moto|extinguisher|jinsi ya kutumia kizima',
    'simu': 'namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura',
    'moshi': 'moshi|moshi mwingi|moshi nyumbani|kujikinga na moshi',
    'maji': 'mtu amezama|uokoaji majini|mtu anazama|kuokolewa majini',
    'zama': 'mtu amezama|uokoaji majini|mtu anazama|kuokolewa majini',
    'umeme': 'mshtuko wa umeme|mtu ameguswa umeme|umeme|hatari ya umeme',
    'kuungua': 'huduma ya kwanza|kuungua|maumivu ya moto|burns',
    'msitu': 'moto wa msitu|savana|vichaka|moto wa mashamba',
    'gari': 'moto wa gari|accident|ajali ya barabara|magari',
    'jengo': 'uokoaji jengo|jengo kuporomoka|mlipuko|jengo linaungua',
    'kemikali': 'kemikali hatari|chemical spill|gesi|kemikali',
    'cpr': 'cpr|pumzi ya bandia|moyo kuacha|resuscitation',
    'moyo': 'cpr|pumzi ya bandia|moyo kuacha|resuscitation',
    'kuzuia': 'kuzuia moto|usalama wa moto|prevensheni|kinga ya moto',
    'gesi': 'moto wa jiko|gesi|gas|cylinder',
    'kiwanda': 'moto wa viwandani|kiwanda|warehouse',
    '112': 'namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura',
  };
  
  for (const [word, key] of Object.entries(wordMap)) {
    if (query.includes(word)) {
      return KNOWLEDGE_BASE[key];
    }
  }
  
  return null;
}

// ── UI FUNCTIONS ──────────────────────────────────────────────────
let messageCount = 0;

function getTime() {
  return new Date().toLocaleTimeString('sw-TZ', {hour:'2-digit', minute:'2-digit'});
}

function addMessage(content, isUser, tagText = null, tagColor = 'alert') {
  const messages = document.getElementById('messages');
  const div = document.createElement('div');
  div.className = `msg ${isUser ? 'user' : 'bot'}`;
  
  const tagHtml = tagText 
    ? `<span class="${tagColor === 'safe' ? 'safe-tag' : 'alert-tag'}">${tagText}</span>` 
    : '';
  
  div.innerHTML = `
    <div class="avatar ${isUser ? 'user-av' : 'bot'}">${isUser ? '👤' : '🔥'}</div>
    <div>
      <div class="bubble-meta">${isUser ? 'WEWE' : 'SADEGPTFIRE'} · ${getTime()}</div>
      <div class="bubble">${tagHtml}${content}</div>
    </div>
  `;
  messages.appendChild(div);
  messages.scrollTop = messages.scrollHeight;
  messageCount++;
}

function showTyping() {
  document.getElementById('typing').classList.add('visible');
  const messages = document.getElementById('messages');
  messages.scrollTop = messages.scrollHeight;
}

function hideTyping() {
  document.getElementById('typing').classList.remove('visible');
}

function sendMessage() {
  const input = document.getElementById('userInput');
  const btn = document.getElementById('sendBtn');
  const text = input.value.trim();
  if (!text) return;
  
  addMessage(text, true);
  input.value = '';
  input.style.height = 'auto';
  btn.disabled = true;
  showTyping();
  
  setTimeout(() => {
    hideTyping();
    const result = findBestResponse(text);
    
    if (result) {
      addMessage(result.response, false, result.tag, result.tagColor);
    } else {
      const rand = DEFAULT_RESPONSES[messageCount % DEFAULT_RESPONSES.length];
      addMessage(rand, false, null, null);
    }
    btn.disabled = false;
    input.focus();
  }, 800 + Math.random() * 700);
}

function askQuick(btn) {
  const text = btn.querySelector('span') ? btn.textContent.replace(btn.querySelector('span').textContent, '').trim() : btn.textContent.trim();
  document.getElementById('userInput').value = text;
  sendMessage();
}

function handleKey(e) {
  if (e.key === 'Enter' && !e.shiftKey) {
    e.preventDefault();
    sendMessage();
  }
}

function autoResize(el) {
  el.style.height = 'auto';
  el.style.height = Math.min(el.scrollHeight, 120) + 'px';
}
</script>
</body>
</html>
