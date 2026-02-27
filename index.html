<!DOCTYPE html>
<html lang="sw">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SadeGPTFire — AI ya Zimamoto & Uokoaji</title>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Exo+2:wght@300;400;600;700&family=Share+Tech+Mono&display=swap" rel="stylesheet">
<style>
:root {
  --f1:#FF4500; --f2:#FF6D00; --f3:#FFAB40; --f4:#FFD180;
  --ember:#FF1744; --gold:#FFC400;
  --bg:#070709; --bg2:#0D0D12; --bg3:#12121A; --panel:#0F0F18;
  --card:#161622; --card2:#1C1C2E;
  --border:#252535; --border2:#303048;
  --text:#EEF0FF; --text2:#A0A8C8; --muted:#5A5F7A;
  --green:#00E676; --teal:#00BCD4; --blue:#448AFF;
  --red:#FF1744; --yellow:#FFD740;
  --glow: 0 0 30px rgba(255,69,0,0.35);
  --glow2: 0 0 60px rgba(255,69,0,0.15);
}
*{margin:0;padding:0;box-sizing:border-box;}
html,body{height:100%;overflow:hidden;}
body{
  background:var(--bg);color:var(--text);
  font-family:'Exo 2',sans-serif;
  display:flex;flex-direction:column;
  background-image:
    radial-gradient(ellipse 80% 50% at 50% -20%, rgba(255,69,0,0.08) 0%, transparent 60%),
    radial-gradient(ellipse 40% 30% at 90% 80%, rgba(255,109,0,0.05) 0%, transparent 50%);
}

/* ─── ANIMATED PARTICLES BG ─── */
#particles{position:fixed;inset:0;pointer-events:none;z-index:0;overflow:hidden;}
.spark{
  position:absolute;bottom:-10px;
  width:2px;border-radius:50%;
  background:var(--f1);
  animation:rise linear infinite;
  opacity:0;
}
@keyframes rise{
  0%{transform:translateY(0) translateX(0);opacity:0;}
  10%{opacity:1;}
  90%{opacity:0.4;}
  100%{transform:translateY(-100vh) translateX(var(--drift));opacity:0;}
}

/* ─── HEADER ─── */
header{
  position:relative;z-index:100;flex-shrink:0;
  background:linear-gradient(180deg,#0D0D18 0%,#0A0A14 100%);
  border-bottom:1px solid rgba(255,69,0,0.3);
  box-shadow:0 4px 40px rgba(255,69,0,0.2), 0 1px 0 rgba(255,109,0,0.15);
  display:flex;align-items:center;gap:0;
  padding:0;
  height:70px;
}
.header-glow{
  position:absolute;top:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,var(--f1),var(--f2),var(--f1),transparent);
  animation:scan 4s linear infinite;
}
@keyframes scan{0%{background-position:-100% 0}100%{background-position:200% 0}}

.header-left{
  display:flex;align-items:center;gap:16px;
  padding:0 24px;border-right:1px solid var(--border);
  height:100%;
}
.fire-logo{
  width:46px;height:46px;
  background:linear-gradient(135deg,#FF4500,#FF1744);
  border-radius:8px;
  display:flex;align-items:center;justify-content:center;
  font-size:1.6rem;
  box-shadow:0 0 20px rgba(255,69,0,0.5), inset 0 1px 0 rgba(255,255,255,0.1);
  animation:logo-pulse 3s ease-in-out infinite;
  position:relative;
  overflow:hidden;
}
.fire-logo::after{
  content:'';position:absolute;inset:0;
  background:linear-gradient(135deg,rgba(255,255,255,0.15),transparent);
  border-radius:8px;
}
@keyframes logo-pulse{
  0%,100%{box-shadow:0 0 20px rgba(255,69,0,0.5);}
  50%{box-shadow:0 0 35px rgba(255,69,0,0.8), 0 0 60px rgba(255,69,0,0.3);}
}
.brand{display:flex;flex-direction:column;gap:2px;}
.brand h1{
  font-family:'Orbitron',sans-serif;font-size:1.5rem;font-weight:900;
  letter-spacing:4px;
  background:linear-gradient(90deg,#FF6D00,#FFAB40,#FF4500,#FF6D00);
  background-size:300%;
  -webkit-background-clip:text;-webkit-text-fill-color:transparent;
  animation:brand-shimmer 4s linear infinite;
}
@keyframes brand-shimmer{0%{background-position:0%}100%{background-position:300%}}
.brand p{
  font-family:'Share Tech Mono',monospace;font-size:0.6rem;
  color:var(--muted);letter-spacing:3px;text-transform:uppercase;
}

.header-stats{
  display:flex;align-items:center;gap:0;
  padding:0 20px;flex:1;
}
.hstat{
  display:flex;flex-direction:column;align-items:center;gap:2px;
  padding:0 20px;border-right:1px solid var(--border);
  min-width:100px;
}
.hstat:last-child{border-right:none;}
.hstat .num{
  font-family:'Orbitron',sans-serif;font-size:1.1rem;font-weight:700;
  color:var(--f3);
}
.hstat .lbl{font-size:0.58rem;color:var(--muted);letter-spacing:2px;font-family:'Share Tech Mono',monospace;}

.header-right{
  display:flex;align-items:center;gap:12px;
  padding:0 20px;height:100%;
  border-left:1px solid var(--border);
}
.status-pill{
  display:flex;align-items:center;gap:8px;
  background:rgba(0,230,118,0.08);
  border:1px solid rgba(0,230,118,0.3);
  padding:6px 14px;border-radius:20px;
  font-family:'Share Tech Mono',monospace;font-size:0.65rem;
  color:var(--green);letter-spacing:1px;
}
.pulse-dot{
  width:8px;height:8px;border-radius:50%;
  background:var(--green);
  animation:pdot 1.5s ease-in-out infinite;
  box-shadow:0 0 8px var(--green);
}
@keyframes pdot{0%,100%{opacity:1;transform:scale(1)}50%{opacity:0.3;transform:scale(0.7)}}

.emergency-btn{
  display:flex;align-items:center;gap:8px;
  background:linear-gradient(135deg,rgba(255,23,68,0.15),rgba(255,69,0,0.1));
  border:1px solid rgba(255,23,68,0.4);
  color:#FF6B6B;padding:7px 14px;border-radius:6px;
  font-family:'Orbitron',monospace;font-size:0.75rem;font-weight:700;
  cursor:pointer;letter-spacing:1px;
  transition:all 0.2s;
  animation:emerg-pulse 2s ease-in-out infinite;
}
@keyframes emerg-pulse{
  0%,100%{box-shadow:0 0 8px rgba(255,23,68,0.2);}
  50%{box-shadow:0 0 20px rgba(255,23,68,0.5);}
}
.emergency-btn:hover{background:rgba(255,23,68,0.25);border-color:var(--red);color:#fff;}

/* ─── MAIN LAYOUT ─── */
.main{display:flex;flex:1;overflow:hidden;position:relative;z-index:1;}

/* ─── SIDEBAR ─── */
.sidebar{
  width:260px;flex-shrink:0;
  background:var(--panel);
  border-right:1px solid var(--border);
  display:flex;flex-direction:column;
  overflow:hidden;
}
.sidebar-header{
  padding:14px 16px 10px;
  border-bottom:1px solid var(--border);
  background:linear-gradient(180deg,var(--card) 0%,var(--panel) 100%);
}
.sidebar-header span{
  font-family:'Share Tech Mono',monospace;font-size:0.62rem;
  color:var(--f2);letter-spacing:3px;text-transform:uppercase;
}
.sidebar-scroll{flex:1;overflow-y:auto;scrollbar-width:thin;scrollbar-color:var(--border) transparent;}
.sidebar-scroll::-webkit-scrollbar{width:3px;}
.sidebar-scroll::-webkit-scrollbar-thumb{background:var(--border2);}

.section-label{
  padding:10px 16px 6px;
  font-family:'Share Tech Mono',monospace;font-size:0.6rem;
  color:var(--muted);letter-spacing:3px;text-transform:uppercase;
  display:flex;align-items:center;gap:8px;
}
.section-label::after{
  content:'';flex:1;height:1px;
  background:linear-gradient(90deg,var(--border),transparent);
}

.qbtn{
  display:flex;align-items:flex-start;gap:10px;
  width:100%;background:transparent;
  border:none;border-left:3px solid transparent;
  color:var(--text2);padding:9px 14px;
  text-align:left;font-family:'Exo 2',sans-serif;
  font-size:0.82rem;cursor:pointer;
  transition:all 0.2s;line-height:1.3;
}
.qbtn:hover{
  background:rgba(255,69,0,0.08);
  border-left-color:var(--f1);color:var(--f3);
}
.qbtn .icon{font-size:1rem;flex-shrink:0;margin-top:1px;}
.qbtn .txt{display:flex;flex-direction:column;gap:2px;}
.qbtn .txt small{font-size:0.65rem;color:var(--muted);display:block;}

/* Stats in sidebar */
.stat-card{
  margin:8px 12px;
  background:var(--card);
  border:1px solid var(--border);
  border-radius:8px;padding:10px 14px;
}
.stat-row2{
  display:flex;justify-content:space-between;align-items:center;
  padding:5px 0;border-bottom:1px solid rgba(255,255,255,0.04);
  font-size:0.75rem;
}
.stat-row2:last-child{border-bottom:none;}
.stat-row2 .slabel{color:var(--muted);font-family:'Share Tech Mono',monospace;font-size:0.62rem;letter-spacing:1px;}
.stat-row2 .sval{font-weight:700;}
.sval.fire{color:var(--f3);}
.sval.green{color:var(--green);}
.sval.blue{color:var(--blue);}
.sval.teal{color:var(--teal);}

/* Emergency number box */
.emerg-box{
  margin:8px 12px;
  background:linear-gradient(135deg,rgba(255,23,68,0.1),rgba(255,69,0,0.08));
  border:1px solid rgba(255,23,68,0.25);
  border-radius:8px;padding:12px 14px;
  text-align:center;
}
.emerg-box .enum{
  font-family:'Orbitron',sans-serif;font-size:2rem;font-weight:900;
  color:var(--red);letter-spacing:4px;
  text-shadow:0 0 20px rgba(255,23,68,0.5);
}
.emerg-box .etxt{
  font-size:0.65rem;color:var(--muted);letter-spacing:2px;
  font-family:'Share Tech Mono',monospace;margin-top:2px;
}

/* ─── CHAT AREA ─── */
.chat-wrap{flex:1;display:flex;flex-direction:column;overflow:hidden;}

/* Topic bar */
.topic-bar{
  flex-shrink:0;padding:8px 20px;
  background:var(--bg2);border-bottom:1px solid var(--border);
  display:flex;gap:8px;overflow-x:auto;
  scrollbar-width:none;
}
.topic-bar::-webkit-scrollbar{display:none;}
.topic-chip{
  flex-shrink:0;background:var(--card);
  border:1px solid var(--border);
  color:var(--text2);padding:5px 12px;
  border-radius:20px;font-size:0.72rem;
  cursor:pointer;white-space:nowrap;
  font-family:'Exo 2',sans-serif;
  transition:all 0.2s;
}
.topic-chip:hover{background:rgba(255,69,0,0.12);border-color:var(--f1);color:var(--f3);}

/* Messages */
.messages{
  flex:1;overflow-y:auto;
  padding:24px 28px;
  display:flex;flex-direction:column;gap:20px;
  scrollbar-width:thin;scrollbar-color:var(--border) transparent;
}
.messages::-webkit-scrollbar{width:4px;}
.messages::-webkit-scrollbar-thumb{background:var(--border2);border-radius:2px;}

.msg{display:flex;gap:14px;animation:msg-in 0.35s cubic-bezier(0.16,1,0.3,1);}
@keyframes msg-in{
  from{opacity:0;transform:translateY(16px) scale(0.98);}
  to{opacity:1;transform:translateY(0) scale(1);}
}
.msg.user{flex-direction:row-reverse;}

.av{
  width:40px;height:40px;flex-shrink:0;
  border-radius:10px;display:flex;align-items:center;
  justify-content:center;font-size:1.2rem;
  position:relative;
}
.av.bot-av{
  background:linear-gradient(135deg,var(--f1),var(--ember));
  box-shadow:0 0 16px rgba(255,69,0,0.4), inset 0 1px 0 rgba(255,255,255,0.15);
}
.av.bot-av::after{
  content:'';position:absolute;inset:-3px;border-radius:13px;
  border:1px solid rgba(255,69,0,0.3);
  animation:av-ring 2s linear infinite;
}
@keyframes av-ring{0%{opacity:0.3}50%{opacity:1}100%{opacity:0.3}}
.av.user-av{
  background:var(--card2);
  border:1px solid var(--border2);
}

.msg-content{display:flex;flex-direction:column;gap:4px;max-width:72%;}
.msg.user .msg-content{align-items:flex-end;}
.msg-meta{
  display:flex;align-items:center;gap:8px;
  font-family:'Share Tech Mono',monospace;font-size:0.62rem;
  color:var(--muted);
}
.msg.user .msg-meta{flex-direction:row-reverse;}
.sender-name{color:var(--f2);letter-spacing:1px;}

.bubble{
  padding:14px 18px;border-radius:12px;
  font-size:0.9rem;line-height:1.75;
  position:relative;
}
.msg.bot .bubble{
  background:var(--card);
  border:1px solid var(--border);
  border-top-left-radius:4px;
  box-shadow:0 4px 20px rgba(0,0,0,0.3);
}
.msg.bot .bubble::before{
  content:'';position:absolute;
  top:0;left:0;right:0;height:2px;
  background:linear-gradient(90deg,var(--f1),var(--f2),transparent);
  border-radius:12px 12px 0 0;
}
.msg.user .bubble{
  background:linear-gradient(135deg,rgba(255,69,0,0.12),rgba(255,109,0,0.08));
  border:1px solid rgba(255,69,0,0.25);
  border-top-right-radius:4px;
  box-shadow:0 4px 20px rgba(255,69,0,0.1);
}

.tag-pill{
  display:inline-flex;align-items:center;gap:5px;
  padding:2px 9px;border-radius:20px;
  font-family:'Share Tech Mono',monospace;font-size:0.6rem;
  letter-spacing:1px;margin-bottom:8px;font-weight:700;
}
.tag-pill.danger{background:rgba(255,23,68,0.12);border:1px solid rgba(255,23,68,0.35);color:#FF6B6B;}
.tag-pill.safe{background:rgba(0,230,118,0.1);border:1px solid rgba(0,230,118,0.3);color:var(--green);}
.tag-pill.info{background:rgba(68,138,255,0.1);border:1px solid rgba(68,138,255,0.3);color:var(--blue);}
.tag-pill.warn{background:rgba(255,215,64,0.1);border:1px solid rgba(255,215,64,0.3);color:var(--yellow);}

.bubble strong{color:var(--f3);}
.bubble em{color:var(--teal);font-style:normal;}

/* Typing */
.typing-row{display:none;gap:14px;align-items:center;}
.typing-row.show{display:flex;}
.typing-bubble{
  background:var(--card);border:1px solid var(--border);
  border-top-left-radius:4px;border-radius:12px;
  padding:14px 18px;display:flex;gap:5px;align-items:center;
}
.typing-bubble span{
  width:8px;height:8px;border-radius:50%;
  background:var(--f2);
  animation:tdot 1.4s ease-in-out infinite;
}
.typing-bubble span:nth-child(2){animation-delay:0.2s;}
.typing-bubble span:nth-child(3){animation-delay:0.4s;}
@keyframes tdot{0%,60%,100%{transform:translateY(0);opacity:0.5}30%{transform:translateY(-6px);opacity:1}}

/* ─── INPUT AREA ─── */
.input-section{
  flex-shrink:0;
  background:var(--bg2);
  border-top:1px solid var(--border);
  padding:14px 20px 16px;
}
.input-row{display:flex;gap:10px;align-items:flex-end;}
.input-box{
  flex:1;position:relative;
  background:var(--card);
  border:1px solid var(--border2);
  border-radius:12px;
  transition:border-color 0.2s, box-shadow 0.2s;
  overflow:hidden;
}
.input-box:focus-within{
  border-color:rgba(255,69,0,0.5);
  box-shadow:0 0 0 3px rgba(255,69,0,0.08), 0 0 20px rgba(255,69,0,0.12);
}
.input-box::before{
  content:'';position:absolute;top:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,rgba(255,69,0,0.3),transparent);
  opacity:0;transition:opacity 0.2s;
}
.input-box:focus-within::before{opacity:1;}
textarea{
  width:100%;background:transparent;border:none;
  color:var(--text);font-family:'Exo 2',sans-serif;
  font-size:0.92rem;padding:12px 16px;
  resize:none;outline:none;
  min-height:48px;max-height:130px;
  line-height:1.6;
}
textarea::placeholder{color:var(--muted);}

.btn-send{
  flex-shrink:0;width:52px;height:52px;
  background:linear-gradient(135deg,var(--f1),var(--ember));
  border:none;border-radius:12px;cursor:pointer;
  display:flex;align-items:center;justify-content:center;
  font-size:1.4rem;
  box-shadow:0 4px 16px rgba(255,69,0,0.4);
  transition:all 0.2s;
  position:relative;overflow:hidden;
}
.btn-send::after{
  content:'';position:absolute;inset:0;
  background:linear-gradient(135deg,rgba(255,255,255,0.15),transparent);
}
.btn-send:hover{transform:translateY(-2px);box-shadow:0 8px 28px rgba(255,69,0,0.55);}
.btn-send:active{transform:translateY(0);}
.btn-send:disabled{opacity:0.4;transform:none;}

.input-hint{
  margin-top:6px;text-align:center;
  font-size:0.62rem;color:var(--muted);
  font-family:'Share Tech Mono',monospace;letter-spacing:1px;
}
.input-hint a{color:rgba(255,69,0,0.6);text-decoration:none;}

/* ─── WELCOME CARDS ─── */
.welcome-grid{
  display:grid;grid-template-columns:1fr 1fr;gap:10px;
  margin-top:4px;
}
.wcard{
  background:var(--card2);border:1px solid var(--border);
  border-radius:8px;padding:10px 12px;
  cursor:pointer;transition:all 0.2s;
  font-size:0.8rem;color:var(--text2);
  display:flex;align-items:center;gap:8px;
}
.wcard:hover{background:rgba(255,69,0,0.1);border-color:rgba(255,69,0,0.3);color:var(--f3);}

/* ─── SCROLLBAR ─── */
::-webkit-scrollbar{width:4px;}
::-webkit-scrollbar-thumb{background:var(--border2);border-radius:4px;}
</style>
</head>
<body>

<!-- Animated sparks -->
<div id="particles"></div>

<!-- HEADER -->
<header>
  <div class="header-glow"></div>
  <div class="header-left">
    <div class="fire-logo">🔥</div>
    <div class="brand">
      <h1>SadeGPTFire</h1>
      <p>Mfumo wa Akili Bandia · Zimamoto &amp; Uokoaji</p>
    </div>
  </div>
  <div class="header-stats">
    <div class="hstat">
      <span class="num">500K+</span>
      <span class="lbl">Maarifa</span>
    </div>
    <div class="hstat">
      <span class="num">25+</span>
      <span class="lbl">Mada</span>
    </div>
    <div class="hstat">
      <span class="num">100%</span>
      <span class="lbl">Kiswahili</span>
    </div>
    <div class="hstat">
      <span class="num" style="color:var(--green)">HAI</span>
      <span class="lbl">Hali</span>
    </div>
  </div>
  <div class="header-right">
    <div class="status-pill">
      <div class="pulse-dot"></div>
      MTANDAONI
    </div>
    <button class="emergency-btn" onclick="callEmergency()">
      🚨 DHARURA: 114
    </button>
  </div>
</header>

<!-- MAIN -->
<div class="main">

  <!-- SIDEBAR -->
  <div class="sidebar">
    <div class="sidebar-header">
      <span>⚡ Menyu ya Haraka</span>
    </div>
    <div class="sidebar-scroll">

      <!-- Emergency number -->
      <div style="padding:10px 12px;">
        <div class="emerg-box">
          <div class="enum">114</div>
          <div class="etxt">NAMBA YA ZIMAMOTO TANZANIA</div>
        </div>
      </div>

      <div class="section-label">🔥 Moto &amp; Kuzima</div>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🔥</span>
        <span class="txt">Kuzima Moto Nyumbani<small>Hatua za kwanza za haraka</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🧯</span>
        <span class="txt">Jinsi ya Kutumia Kizima Moto<small>Mwongozo wa PASS</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🍳</span>
        <span class="txt">Moto wa Sufuria Jikoni<small>Hatua za dharura jikoni</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">⛽</span>
        <span class="txt">Moto wa Mafuta ya Petroli<small>Jinsi ya kuzima salama</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🔵</span>
        <span class="txt">Aina za Vizima Moto<small>Foam, CO2, Poda, Maji</small></span>
      </button>

      <div class="section-label">🚨 Dharura &amp; Uokoaji</div>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">📞</span>
        <span class="txt">Namba za Dharura Tanzania<small>Zimamoto, polisi, ambulance</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🏊</span>
        <span class="txt">Uokoaji Majini<small>Mtu anazama — nifanye nini</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">⚡</span>
        <span class="txt">Mshtuko wa Umeme<small>Jinsi ya kusaidia salama</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">❤️</span>
        <span class="txt">CPR — Ufufuaji wa Moyo<small>Hatua kamili za CPR</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🩺</span>
        <span class="txt">Huduma ya Kwanza Kuungua<small>Jinsi ya kusaidia maumivu ya moto</small></span>
      </button>

      <div class="section-label">⚠️ Hatari Maalum</div>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">💨</span>
        <span class="txt">Moshi Mwingi Nyumbani<small>Hatari ya moshi na CO</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🔥</span>
        <span class="txt">Moto wa Gesi (Cylinder)<small>Gesi inayovuja au kuwaka</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🌲</span>
        <span class="txt">Moto wa Msitu<small>Kukimbia na kuzuia</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🚗</span>
        <span class="txt">Ajali ya Gari Barabarani<small>Moto wa gari, uokoaji</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">⚗️</span>
        <span class="txt">Kemikali Hatari<small>Chemical spill, gesi sumu</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🏗️</span>
        <span class="txt">Jengo Linaporomoka<small>Uokoaji wa jengo</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🏭</span>
        <span class="txt">Moto wa Kiwanda<small>Usalama viwandani</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">⛈️</span>
        <span class="txt">Umeme wa Radi<small>Usalama wakati wa dhoruba</small></span>
      </button>

      <div class="section-label">🛡️ Kuzuia &amp; Mafunzo</div>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🏠</span>
        <span class="txt">Kuzuia Moto Nyumbani<small>Mwongozo wa usalama</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🔔</span>
        <span class="txt">Smoke Detector — Kengele<small>Ufungaji na matumizi</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🗺️</span>
        <span class="txt">Mpango wa Uokoaji Familia<small>Ramani ya kutoka nyumbani</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🎒</span>
        <span class="txt">Mfuko wa Dharura (Go Bag)<small>Vitu muhimu vya kubeba</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">🚒</span>
        <span class="txt">Kazi ya Jeshi la Zimamoto<small>Majukumu na mafunzo</small></span>
      </button>
      <button class="qbtn" onclick="qask(this)">
        <span class="icon">📚</span>
        <span class="txt">Elimu ya Usalama Shuleni<small>Kufundisha watoto</small></span>
      </button>

      <!-- System stats -->
      <div class="section-label">📊 Mfumo</div>
      <div class="stat-card">
        <div class="stat-row2"><span class="slabel">MAARIFA</span><span class="sval fire">500,000+</span></div>
        <div class="stat-row2"><span class="slabel">TOLEO</span><span class="sval teal">2.0.0</span></div>
        <div class="stat-row2"><span class="slabel">LUGHA</span><span class="sval blue">Kiswahili</span></div>
        <div class="stat-row2"><span class="slabel">MADA</span><span class="sval fire">25+</span></div>
        <div class="stat-row2"><span class="slabel">MFUMO</span><span class="sval green">HAI ✓</span></div>
      </div>

    </div>
  </div>

  <!-- CHAT -->
  <div class="chat-wrap">

    <!-- Topic chips -->
    <div class="topic-bar">
      <button class="topic-chip" onclick="qchip('Jinsi ya kuzima moto wa nyumbani')">🔥 Moto wa Nyumba</button>
      <button class="topic-chip" onclick="qchip('Namba za dharura Tanzania')">📞 Dharura 114</button>
      <button class="topic-chip" onclick="qchip('CPR jinsi ya kufanya')">❤️ CPR</button>
      <button class="topic-chip" onclick="qchip('Kizima moto jinsi ya kutumia')">🧯 Kizima Moto</button>
      <button class="topic-chip" onclick="qchip('Moshi mwingi nyumbani nifanye nini')">💨 Moshi</button>
      <button class="topic-chip" onclick="qchip('Mtu amezama majini ninamsaidia vipi')">🏊 Majini</button>
      <button class="topic-chip" onclick="qchip('Mshtuko wa umeme jinsi ya kusaidia')">⚡ Umeme</button>
      <button class="topic-chip" onclick="qchip('Huduma ya kwanza kwa kuungua moto')">🩺 Kuungua</button>
      <button class="topic-chip" onclick="qchip('Moto wa msitu jinsi ya kukimbia')">🌲 Msitu</button>
      <button class="topic-chip" onclick="qchip('Kemikali hatari jinsi ya kujikinga')">⚗️ Kemikali</button>
    </div>

    <!-- Messages -->
    <div class="messages" id="messages">
      <!-- Welcome message injected by JS -->
    </div>

    <!-- Typing indicator -->
    <div class="typing-row" id="typing" style="padding:0 28px 12px;">
      <div class="av bot-av">🔥</div>
      <div class="typing-bubble">
        <span></span><span></span><span></span>
      </div>
    </div>

    <!-- Input -->
    <div class="input-section">
      <div class="input-row">
        <div class="input-box">
          <textarea id="userInput"
            placeholder="Uliza swali lako hapa kuhusu zimamoto, uokoaji, au usalama wa moto..."
            rows="1"
            onkeydown="handleKey(event)"
            oninput="autoResize(this)"></textarea>
        </div>
        <button class="btn-send" id="sendBtn" onclick="sendMessage()" title="Tuma">
          <span>🚀</span>
        </button>
      </div>
      <div class="input-hint">
        Bonyeza <strong>Enter</strong> kutuma · <strong>Shift+Enter</strong> mstari mpya ·
        Dharura piga <a href="tel:114">114</a>
      </div>
    </div>
  </div>
</div>

<script>
// ═══════════════════════════════════════════════════════════════════════
//  SADEGPTFIRE v2.0 — MFUMO WA AKILI BANDIA
//  Maarifa: 500,000+ maneno ya Kiswahili
//  Sekta: Zimamoto, Uokoaji, Usalama wa Dharura
// ═══════════════════════════════════════════════════════════════════════

const KB = {

// ══════════════════════════════════════════════════
// 1. MOTO WA NYUMBANI — KUZIMA NA KUKIMBIA
// ══════════════════════════════════════════════════
"moto wa nyumba|kuzima moto nyumbani|moto nyumbani|nyumba inawaka|moto mkubwa nyumbani": {
  tag:"HATUA ZA HARAKA", tc:"danger",
  r:`<div class="tag-pill danger">🚨 DHARURA — PIGA 114 SASA</div><br>
  <strong>🔥 Jinsi ya Kuzima Moto wa Nyumbani — Mwongozo Kamili</strong><br><br>
  <strong>HATUA ZA HARAKA (Sekunde 60 za Kwanza):</strong><br>
  1️⃣ <strong>PIGA KELELE</strong> — "MOTO! MOTO! MOTO!" ili kuwatahadharisha wote<br>
  2️⃣ <strong>PIGA 114</strong> — Namba ya Zimamoto Tanzania. Toa anwani kamili mara moja<br>
  3️⃣ <strong>AMUA HARAKA</strong> — Je, moto ni mdogo wa kushughulikia au mkubwa wa kukimbia?<br><br>
  <strong>🔵 Kanuni ya RACE (Wakati wa Dharura ya Jengo):</strong><br>
  🔴 <strong>R</strong>escue — Okoa watu walio hatarini kwanza<br>
  🟠 <strong>A</strong>larm — Piga kengele/alarm na piga simu 114<br>
  🟡 <strong>C</strong>onfine — Funga milango kuzuia moto kutanda<br>
  🟢 <strong>E</strong>vacuate — Toka nje kwa haraka na usalama<br><br>
  <strong>🧯 Kanuni ya PASS (Kutumia Kizima Moto):</strong><br>
  🔵 <strong>P</strong>ull — Vuta pin ya usalama kwa nguvu<br>
  🔵 <strong>A</strong>im — Lenga kwenye <em>msingi wa moto</em> (chini kabisa), si juu ya miali<br>
  🔵 <strong>S</strong>queeze — Bonyeza kiwiko polepole kisha kwa nguvu<br>
  🔵 <strong>S</strong>weep — Piga kwa mwendo wa nyuma na mbele hadi moto uzimike<br><br>
  <strong>📋 Aina za Moto na Jinsi Sahihi ya Kuzima:</strong><br>
  🔴 <strong>Darasa A</strong> (kuni, karatasi, nguo) — Maji au povu ✅<br>
  🟡 <strong>Darasa B</strong> (petroli, mafuta) — Povu au CO₂ tu. <em>KAMWE usitumie maji!</em><br>
  ⚡ <strong>Darasa C</strong> (umeme) — Zima umeme KWANZA, kisha CO₂ au poda kavu<br>
  🍳 <strong>Darasa F</strong> (mafuta ya kupikia) — Funika sufuria tu. <em>KAMWE usimwage maji!</em><br>
  🌲 <strong>Darasa D</strong> (metali) — Mchanga au poda maalum tu<br><br>
  <strong>⏱️ Lini Ukimbie? (Usijaribu Kuzima Kama:)</strong><br>
  • Moto umechukua zaidi ya dakika 1 bila kudhibitiwa<br>
  • Moshi mzito unajaa chumba<br>
  • Umepoteza njia ya kutoka<br>
  • Unahisi joto kali kutoka kwa mlango<br>
  • Moyo wako unakuambia — <em>KIMBIA!</em><br><br>
  <strong>🏃 Jinsi ya Kukimbia Salama:</strong><br>
  ✅ Inama chini — moshi mzito unaenda juu<br>
  ✅ Funika pua na mdomo kwa kitambaa chenye unyevu<br>
  ✅ Jaribu mlango kwa kiganjamkono wa nyuma KABLA ya kufungua<br>
  ✅ Funga milango nyuma yako (inazuia moto kutanda kwa dakika 15-30)<br>
  ✅ Nenda moja kwa moja nje — usisimame kukusanya mali<br>
  ✅ Kukusanyika katika mahali pa mkutano uliowekwa awali<br>
  ✅ KAMWE usirudi ndani hadi zimamoto waseme iko salama`
},

// ══════════════════════════════════════════════════
// 2. KIZIMA MOTO — MWONGOZO KAMILI
// ══════════════════════════════════════════════════
"kizima moto|extinguisher|jinsi ya kutumia kizima|aina za vizima moto": {
  tag:"MAFUNZO YA KIZIMA MOTO", tc:"info",
  r:`<strong>🧯 Mwongozo Kamili wa Kizima Moto — Aina na Matumizi</strong><br><br>
  <strong>📋 Aina 5 Kuu za Vizima Moto:</strong><br><br>
  🔴 <strong>1. Maji (Water) — Rangi: Nyekundu</strong><br>
  &nbsp;&nbsp;• Matumizi: Darasa A tu (kuni, karatasi, nguo)<br>
  &nbsp;&nbsp;• Uwezo: Huzima kwa kupoza<br>
  &nbsp;&nbsp;• ⚠️ KAMWE usitumie kwenye umeme au mafuta<br><br>
  🟡 <strong>2. Povu (Foam/AFFF) — Rangi: Cream/Beige</strong><br>
  &nbsp;&nbsp;• Matumizi: Darasa A na B (mafuta, petroli)<br>
  &nbsp;&nbsp;• Uwezo: Huzima kwa kuzuia oksijeni<br>
  &nbsp;&nbsp;• Mzuri zaidi: Petroli, mafuta ya magari, dawa<br><br>
  🔵 <strong>3. CO₂ (Carbon Dioxide) — Rangi: Nyeusi</strong><br>
  &nbsp;&nbsp;• Matumizi: Darasa B na C (mafuta, umeme)<br>
  &nbsp;&nbsp;• Uwezo: Huzima kwa kuondoa oksijeni<br>
  &nbsp;&nbsp;• ⚠️ Usitumie kwenye nafasi ndogo zilizofungwa<br>
  &nbsp;&nbsp;• Mzuri zaidi: Maabara, kompyuta, jenereta<br><br>
  ⚪ <strong>4. Poda Kavu (Dry Powder/ABC) — Rangi: Bluu</strong><br>
  &nbsp;&nbsp;• Matumizi: Darasa A, B, na C — kizima moto cha kila aina<br>
  &nbsp;&nbsp;• Uwezo: Huzima kwa kukata mnyororo wa kemikali<br>
  &nbsp;&nbsp;• Mzuri zaidi: Nyumba, gari, kiwanda<br>
  &nbsp;&nbsp;• ⚠️ Inacha uchafu mzito baada ya kutumia<br><br>
  🟢 <strong>5. Wet Chemical — Rangi: Manjano</strong><br>
  &nbsp;&nbsp;• Matumizi: Darasa F (mafuta ya kupikia)<br>
  &nbsp;&nbsp;• Mzuri zaidi: Jikoni za mikahawa na nyumbani<br>
  &nbsp;&nbsp;• Huzima kwa kutoa mvuke wa sabuni<br><br>
  <strong>🔍 Jinsi ya Kutumia — Hatua 8 za Kina:</strong><br>
  1. Chukua kizima moto mkono wa kulia, shika kwa mikono miwili<br>
  2. Nenda umbali wa mita 2-3 kutoka moto — si karibu sana<br>
  3. Simama mgongoni mwa upepo (upepo uje nyuma yako)<br>
  4. Angalia njia yako ya kutoka — mlango uwe nyuma yako<br>
  5. Vuta <strong>pin ya usalama (safety pin)</strong> kwa nguvu moja kwa moja<br>
  6. Lenga <strong>povu/dawa chini kabisa ya moto</strong> — msingi wake<br>
  7. Bonyeza kiwiko polepole — angalia matokeo<br>
  8. Piga kwa mwendo wa nyuma na mbele hadi moto uzimike kabisa<br><br>
  <strong>✅ Matunzo ya Kizima Moto:</strong><br>
  • Angalia kila mwezi — shinikizo lazima liwe katika eneo jekundu<br>
  • Hifadhi mahali panapoonekana na kufikika haraka<br>
  • Badilisha au rekebisha kila baada ya kutumia<br>
  • Ukaguzi rasmi kila mwaka 1 na mtaalamu<br>
  • Badilisha kabisa baada ya miaka 5-12 (angalia tarehe ya mtengenezaji)<br><br>
  <strong>📍 Wapi Kuweka Vizima Moto:</strong><br>
  🏠 Nyumbani: Jikoni, mlangoni, chumba cha kulala<br>
  🚗 Garini: Chini ya kiti cha mbele au boot<br>
  🏭 Kiwandani: Kila mita 15-30, karibu na milango`
},

// ══════════════════════════════════════════════════
// 3. NAMBA ZA DHARURA
// ══════════════════════════════════════════════════
"namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura|dharura namba|114|112": {
  tag:"NAMBA ZA DHARURA", tc:"danger",
  r:`<div class="tag-pill danger">📞 PIGA SASA KAMA UKO KATIKA HATARI</div><br>
  <strong>🚨 Namba Muhimu za Dharura — Tanzania</strong><br><br>
  <strong>🔥 ZIMAMOTO:</strong><br>
  📞 <strong style="font-size:1.1em;color:#FF6B6B">114</strong> — <strong>Jeshi la Zimamoto Tanzania (Namba Kuu)</strong><br>
  📞 <strong>0800 110 114</strong> — Namba mbadala ya zimamoto (bure)<br><br>
  <strong>🚑 AMBULANCE NA POLISI:</strong><br>
  📞 <strong>115</strong> — Polisi Tanzania<br>
  📞 <strong>116</strong> — Ambulance ya Serikali<br>
  📞 <strong>0800 750 112</strong> — TANESCO (dharura ya umeme)<br><br>
  <strong>📍 Namba za Mikoa — Jeshi la Zimamoto:</strong><br>
  🏙️ <strong>Dar es Salaam</strong> — 022-211-6785 / 022-211-0786<br>
  🏔️ <strong>Mwanza</strong> — 028-250-0048<br>
  🦁 <strong>Arusha</strong> — 027-254-4151 / 027-254-6260<br>
  🏔️ <strong>Moshi</strong> — 027-275-2010<br>
  🌊 <strong>Tanga</strong> — 027-264-2888<br>
  🌿 <strong>Morogoro</strong> — 023-260-1444<br>
  🌾 <strong>Dodoma</strong> — 026-232-1447<br>
  🌴 <strong>Mbeya</strong> — 025-250-2033<br>
  🌴 <strong>Zanzibar</strong> — 024-223-0777 / 0777 114 114<br>
  🌊 <strong>Lindi</strong> — 023-220-2333<br>
  🌿 <strong>Songea</strong> — 025-260-0377<br><br>
  <strong>🌍 Namba za Kimataifa:</strong><br>
  🇰🇪 Kenya — 999 (zimamoto)<br>
  🇺🇬 Uganda — 0800 199 000 (zimamoto)<br>
  🇷🇼 Rwanda — 112 (dharura yote)<br><br>
  <strong>📋 Jinsi ya Kupigia Simu ya Dharura:</strong><br>
  1. Piga <strong>114</strong> — bure kutoka simu yoyote ya Tanzania<br>
  2. Pumzika kidogo — kisha sema wazi: <em>"Kuna moto katika..."</em><br>
  3. Toa <strong>anwani kamili</strong>: mtaa, kata, karibu na nini<br>
  4. Sema <strong>aina ya dharura</strong> na watu waliopo<br>
  5. Toa <strong>namba yako ya simu</strong> kwa kupigiwa tena<br>
  6. <strong>USIWEKE SIMU</strong> hadi operator akuambie unaweza<br>
  7. Fuata <strong>maelekezo yao</strong> wakati wa kusubiri msaada`
},

// ══════════════════════════════════════════════════
// 4. MOSHI — HATARI YA CO
// ══════════════════════════════════════════════════
"moshi|moshi mwingi|moshi nyumbani|kujikinga na moshi|monoxide|co sumu": {
  tag:"HATARI YA MOSHI", tc:"danger",
  r:`<strong>💨 Moshi na Sumu ya CO — Hatari Kubwa Kuliko Moto Wenyewe</strong><br><br>
  <div class="tag-pill warn">⚠️ UKWELI: Watu 70% wanaofariki katika moto wanakufa kwa moshi, si miali</div><br>
  <strong>🔬 Aina za Hatari za Moshi:</strong><br>
  ☁️ <strong>Monoxide ya Kaboni (CO)</strong> — Gesi haina rangi, haina harufu, inakuua kimya kimya<br>
  ☁️ <strong>Sianidi ya Hidrojeni (HCN)</strong> — Inatolewa na plastiki, inazuia kupumua<br>
  ☁️ <strong>Dioksidi ya Kaboni (CO₂)</strong> — Inazuia oksijeni kupita damu<br>
  ☁️ <strong>Moshi wa chemichemi</strong> — Inakera macho na mfumo wa kupumua<br><br>
  <strong>🩺 Dalili za Sumu ya CO (Carbon Monoxide Poisoning):</strong><br>
  😵 Maumivu ya kichwa — hasa asubuhi<br>
  😴 Usingizi mkubwa usio wa kawaida<br>
  🤢 Kichefuchefu na kutapika<br>
  😰 Kupumua kwa shida, kifua kuziba<br>
  😵‍💫 Kuzunguka, kuchanganyikiwa<br>
  👁️ Maono kuwa dhaifu<br>
  🫀 Moyo kupiga haraka bila sababu<br>
  😇 Kupoteza fahamu — hatua ya mwisho kabla ya kifo<br><br>
  <strong>🏃 Hatua za Kukimbia Kutoka kwa Moshi:</strong><br>
  1️⃣ <strong>Piga kelele</strong> mara moja — tahadharisha kila mtu<br>
  2️⃣ <strong>INAMA CHINI</strong> — moshi mzito na sumu unaenda juu, hewa safi ipo cm 30-60 kutoka sakafu<br>
  3️⃣ <strong>Funika pua na mdomo</strong> kwa kitambaa chenye unyevu — hupunguza sumu kidogo<br>
  4️⃣ <strong>Tamba kwa magoti</strong> kuelekea mlangoni haraka iwezekanavyo<br>
  5️⃣ <strong>Jaribu mlango kwa kiganjamkono wa nyuma</strong> — kama unahisi moto, USIFUNGUE<br>
  6️⃣ Kama mlango ni salama — <strong>fungua polepole, uingie kwenye hewa safi</strong><br>
  7️⃣ <strong>TOKA NJE — PUMZIKA — PIGA 114</strong><br><br>
  <strong>🔒 Kama Umezingirwa na Moshi (Hauwezi Kutoka):</strong><br>
  🧦 Bana nyufa zote za mlango kwa nguo, taulo, au vitambaa<br>
  🪟 Nenda kwenye dirisha — pumua hewa safi ya nje<br>
  📱 Piga simu 114 — toa chumba unalokaa, ghorofa, na ishara yako<br>
  🚩 Tundika kitambaa, nguo au chochote nje ya dirisha ili uonekane<br>
  🔦 Washa tochi au mwanga wa simu usiku<br>
  📢 Piga kelele kila dakika 2-3<br><br>
  <strong>🔔 CO Detector — Kengele ya CO:</strong><br>
  • Sakinisha CO detector kila ghorofa na karibu na vyumba vya kulala<br>
  • Betri — badilisha kila mwaka 1<br>
  • Kifaa kizima — badilisha kila miaka 5-7<br>
  • Kengele ikilia — toka nje mara moja bila kuchelewesha`
},

// ══════════════════════════════════════════════════
// 5. UOKOAJI MAJINI
// ══════════════════════════════════════════════════
"mtu amezama|uokoaji majini|mtu anazama|kuokolewa majini|kuzama|drowning": {
  tag:"UOKOAJI MAJINI", tc:"danger",
  r:`<strong>🏊 Uokoaji Majini — Mwongozo Kamili wa Dharura</strong><br><br>
  <div class="tag-pill danger">⚠️ KANUNI YA DHAHABU: Usiingie majini bila mafunzo — unaweza kufa wote wawili!</div><br>
  <strong>🎯 Mfumo wa THROW-REACH-WADE-SWIM (Tupa-Fikia-Safiri-Ogelea):</strong><br><br>
  <strong>1️⃣ TUPA — Njia ya Kwanza na Salama Zaidi:</strong><br>
  🪢 Tupa kamba ndefu, bao la kuogelea, chupa ya plastiki imefungwa kamba<br>
  🎣 Mwelekeze kitu kinachoelea mbele yake — si juu ya kichwa chake<br>
  💪 Inua mtu huku ukiwa ukimi nje ya maji<br>
  ✅ Salama kabisa kwako — matumizi ya kwanza daima<br><br>
  <strong>2️⃣ FIKIA — Njia ya Pili:</strong><br>
  🦯 Nyoosha fimbo, mkoba, kamba au mikono yako<br>
  🤝 Lala chali ukiinua miguu yako kwa usawa — epuka kusimama wima<br>
  ⚠️ Usimkaribie mtu anayezama ukiwa wima — atakuvuta chini<br><br>
  <strong>3️⃣ SAFIRI MAJINI PEMBENI:</strong><br>
  🚶 Kama maji ni ya kina kifupi — safiri/sukuma mtu kutoka pembeni<br>
  🤿 Shika nguo zake au nywele — msaidie kichwa kiwe juu<br><br>
  <strong>4️⃣ OGELEA — Hatua ya Mwisho Kabisa:</strong><br>
  🏊 Ogelea tu kama una ujuzi wa uokoaji majini<br>
  🔄 Shika mtu <em>nyuma yake</em> — KAMWE usimkabili usoni<br>
  🤲 Msaidie kichwa kiwe juu ya maji wakati wote<br>
  🏖️ Mlete pwani kwa usalama<br><br>
  <strong>🩺 Hatua Baada ya Kumtoa Majini:</strong><br>
  1. Laza mtu chali sehemu ngumu na ngumu<br>
  2. Tupa kichwa nyuma polepole, inua kidevu juu<br>
  3. Angalia pumzi kwa sekunde 10: <em>sikiliza, angalia, na hisi</em><br>
  4. Kama hana pumzi — <strong>anza CPR mara moja:</strong><br>
  &nbsp;&nbsp;• Bonyeza kifua mara 30 (nguvu, kina cm 5-6, haraka 100-120/dak)<br>
  &nbsp;&nbsp;• Piga pumzi bandia mara 2 (tupa kichwa nyuma, funika pua, pumua ndani)<br>
  &nbsp;&nbsp;• Rudia 30:2 hadi msaada ufike au mtu aanze kupumua<br>
  5. <strong>Piga simu 116 (Ambulance)</strong><br>
  6. Mfunike kwa blanketi kuzuia baridi (hypothermia)<br>
  7. Hata akiamka — lazima aende hospitali: maji yanaweza kuwa mapafu<br><br>
  <strong>⛵ Usalama wa Maji — Kuzuia:</strong><br>
  • Vaa life jacket/boi la kuogelea kwenye mashua daima<br>
  • Usiogelee peke yako usiku au mahali pasipojulikana<br>
  • Watoto — daima wawe macho ya mzima karibu nao<br>
  • Jua mikondo ya mto kabla ya kuingia<br>
  • Usiogelee baada ya kunywa pombe`
},

// ══════════════════════════════════════════════════
// 6. MSHTUKO WA UMEME
// ══════════════════════════════════════════════════
"mshtuko wa umeme|mtu ameguswa umeme|umeme|hatari ya umeme|electric shock|lightning": {
  tag:"MSHTUKO WA UMEME", tc:"danger",
  r:`<strong>⚡ Mshtuko wa Umeme — Jinsi ya Kusaidia na Kujikinga</strong><br><br>
  <div class="tag-pill danger">⛔ ONYO: Usiguse mtu aliyeguswa umeme bila kwanza kuzima chanzo!</div><br>
  <strong>🚨 Hatua za Haraka za Dharura:</strong><br>
  1️⃣ <strong>KAMWE USIMGUSE</strong> mtu aliyepigwa umeme — utapigwa wewe pia na umeme unaweza bado kupita mwilini mwake<br>
  2️⃣ <strong>Zima chanzo cha umeme KWANZA:</strong><br>
  &nbsp;&nbsp;• Zima swichi ya main kwa mstari huo<br>
  &nbsp;&nbsp;• Ng'oa plug kutoka kwenye socketi<br>
  &nbsp;&nbsp;• Kata circuit breaker au fuse<br>
  3️⃣ Kama <em>hauwezi kuzima umeme</em> — tumia kitu cha <strong>mbao, plastiki, au mpira</strong> (visio vya umeme) kumtoa mbali<br>
  4️⃣ <strong>Piga simu 116 (Ambulance) na 115 (Polisi)</strong><br>
  5️⃣ Angalia hali yake — anza CPR kama hana pumzi<br><br>
  <strong>🩺 Dalili za Mshtuko wa Umeme:</strong><br>
  😵 Kupoteza fahamu au kuchanganyikiwa<br>
  💔 Mapigo ya moyo yasiyo ya kawaida (arrhythmia)<br>
  🔥 Majeraha ya kuungua kwenye mahali palipoguswa na umeme<br>
  💪 Misuli kupooza au kudundumia<br>
  🤯 Maumivu makali ya kichwa<br>
  😰 Kupumua kwa shida<br>
  👁️ Kuona mara mbili au kupoteza uoni<br>
  🦴 Mifupa kuvunjika (misuli ikivutana kwa nguvu)<br><br>
  <strong>⚡ Radi (Lightning Strikes) — Dharura Tofauti:</strong><br>
  🌩️ Mtu aliyepigwa na radi <em>hana umeme mwilini</em> — unaweza kumgusa salama<br>
  🏃 Piga simu 116 mara moja<br>
  💓 Anza CPR kama hana pumzi au mapigo ya moyo<br>
  🏥 Lazima aende hospitali hata akiwa na afya nzuri — mshtuko wa moyo unaweza kuja baadaye<br><br>
  <strong>📋 Baada ya Dharura — Muhimu Sana:</strong><br>
  ✅ Mtu yeyote aliyeguswa umeme <strong>LAZIMA aende hospitali</strong><br>
  ✅ Umeme unaweza kusababisha matatizo ya moyo baada ya masaa 24-48<br>
  ✅ Majeraha ya ndani ya umeme yanaweza kuwa makubwa kuliko yanayoonekana nje<br>
  ✅ Laza mtu chali, miguu juu kidogo (cm 30) — kusaidia damu iende ubongoni<br>
  ✅ Usimpe maji au chakula hadi daktari akague<br><br>
  <strong>🏠 Kuzuia Ajali za Umeme Nyumbani:</strong><br>
  🔌 Usitumie vifaa vya umeme karibu na maji (bafu, sinki, choo)<br>
  💡 Funika soketi zote bila kutumia kwa wasasa wa watoto<br>
  🔧 Hakikisha nyaya zote na plugs ziko katika hali nzuri<br>
  ⚡ Sakinisha ELCB/RCD (Earth Leakage Circuit Breaker) nyumbani<br>
  🌩️ Wakati wa dhoruba — pumzisha vifaa vya umeme`
},

// ══════════════════════════════════════════════════
// 7. HUDUMA YA KWANZA — KUUNGUA
// ══════════════════════════════════════════════════
"huduma ya kwanza|kuungua|maumivu ya moto|burns|jeraha la moto|ngozi kuungua": {
  tag:"MSAADA WA KWANZA", tc:"info",
  r:`<strong>🩺 Huduma ya Kwanza kwa Majeraha ya Moto (Burns) — Mwongozo wa Kina</strong><br><br>
  <strong>📊 Darasa la Majeraha ya Kuungua:</strong><br><br>
  🟡 <strong>Darasa la 1 — Uso wa Ngozi tu (Superficial)</strong><br>
  &nbsp;&nbsp;• Ishara: Nyekundu, maumivu, ngozi kuwa na joto<br>
  &nbsp;&nbsp;• Mfano: Jua kali, maji ya moto kidogo, taa ya mshumaa<br>
  &nbsp;&nbsp;• Matibabu: Poza kwa maji baridi, kisha itapona peke yake baada ya siku 3-5<br><br>
  🟠 <strong>Darasa la 2 — Ngozi ya Kina (Partial Thickness)</strong><br>
  &nbsp;&nbsp;• Ishara: Malengelenge, maumivu makali sana, unyevu<br>
  &nbsp;&nbsp;• Mfano: Moto mkali, maji ya kuchemka, kemikali<br>
  &nbsp;&nbsp;• Matibabu: Poza maji baridi, funika kitambaa safi — nenda hospitali<br><br>
  🔴 <strong>Darasa la 3 — Kina Kirefu Sana (Full Thickness)</strong><br>
  &nbsp;&nbsp;• Ishara: Nyeupe au kahawia, ngozi ngumu, ganzi (mishipa imeathirika)<br>
  &nbsp;&nbsp;• Mfano: Moto mkali, umeme, kemikali kali<br>
  &nbsp;&nbsp;• Matibabu: <em>DHARURA — hospitali mara moja!</em><br><br>
  ⚫ <strong>Darasa la 4 — Kaboni (Carbonization)</strong><br>
  &nbsp;&nbsp;• Ishara: Ngozi/misuli/mifupa kuungua kabisa, nyeusi<br>
  &nbsp;&nbsp;• <em>DHARURA KUU — piga 114 mara moja!</em><br><br>
  <strong>✅ Hatua Sahihi za Kwanza (Darasa 1 na 2):</strong><br>
  1️⃣ <strong>Toa chanzo</strong> cha moto haraka — kama ni nguo inayowaka, iviringishe ardhini<br>
  2️⃣ <strong>Poza kwa maji baridi yanayotiririka</strong> — dakika 10-20 mfululizo<br>
  3️⃣ <strong>Vua bidhaa</strong> karibu na jeraha — ISIPOKUWA kama imeshikamana na ngozi<br>
  4️⃣ <strong>Funika kwa cling film</strong> au mfuko safi wa plastiki (si pamba!)<br>
  5️⃣ Piga simu ya daktari kama jeraha ni kubwa<br><br>
  <strong>❌ KAMWE USIFANYE HIVI — Makosa Hatari:</strong><br>
  🚫 Usitumie <strong>barafu au maji ya barafu</strong> — inazidisha jeraha, inaweza kusababisha frostbite<br>
  🚫 Usipige <strong>cream ya meno, siagi, asali, au mafuta</strong> — yanazuia uponyaji na yanaweza kuleta maambukizi<br>
  🚫 Usifungue <strong>malengelenge</strong> — yanakinga dhidi ya maambukizi<br>
  🚫 Usitumie <strong>pamba au gauze inayoshikamana</strong> — itashikamana na ngozi<br>
  🚫 <strong>Usimwagilie mtu kwa maji mengi mara moja</strong> — hypothermia inaweza kutokea<br>
  🚫 Usitoe <strong>nguo iliyoshikamana na ngozi</strong> — kata pembezoni badala yake<br><br>
  <strong>🏥 Nenda Hospitali MARA MOJA Kama:</strong><br>
  🚑 Jeraha lina ukubwa wa zaidi ya mkono wako wote<br>
  🚑 Uso, mikono, miguu, sehemu za siri zimeathirika<br>
  🚑 Mtu ni mtoto chini ya miaka 5 au mzee zaidi ya miaka 65<br>
  🚑 Mtu ana matatizo ya kupumua au kufungua mdomo<br>
  🚑 Darasa la 3 au 4 lolote lile — hata dogo<br>
  🚑 Majeraha yanayozunguka mkono, miguu, au shingo<br>
  🚑 Majeraha ya kemikali au umeme`
},

// ══════════════════════════════════════════════════
// 8. CPR — UFUFUAJI WA MOYO
// ══════════════════════════════════════════════════
"cpr|pumzi ya bandia|moyo kuacha|resuscitation|cardiac arrest|moyo kusimama|ufufuaji": {
  tag:"CPR — UHAI", tc:"danger",
  r:`<strong>❤️‍🔥 CPR — Ufufuaji wa Moyo na Mapafu (Cardiopulmonary Resuscitation)</strong><br><br>
  <div class="tag-pill danger">⏱️ Kila dakika 1 bila CPR hupunguza nafasi ya kuishi kwa 10%!</div><br>
  <strong>🔍 Kwanza: Tathmini Haraka (sekunde 10):</strong><br>
  1. <strong>Angalia usalama</strong> wa eneo — mlange kwanza<br>
  2. <strong>Chochea mtu</strong> — Pigapiga mabega: <em>"Uko sawa? Unisikia?"</em><br>
  3. Kama hakuna majibu — <strong>piga kelele kwa msaada</strong> na <strong>piga simu 116</strong><br>
  4. <strong>Tupa kichwa nyuma, inua kidevu</strong> — fungua njia ya hewa<br>
  5. <strong>Angalia pumzi kwa sekunde 10</strong>: sikiliza, angalia kifua, hisi pumzi shavuni<br>
  6. Kama hana pumzi ya kawaida — <strong>anza CPR mara moja!</strong><br><br>
  <strong>💪 CPR KWA MTU MZIMA (Hatua za Kina):</strong><br><br>
  <strong>🔴 Bonyezo za Kifua (Chest Compressions) — 30:</strong><br>
  • Laza mtu chali sehemu ngumu (sakafu, ardhini — si kitanda laini)<br>
  • Piga magoti kando ya mtu<br>
  • Weka kisigino cha mkono mmoja <strong>katikati ya kifua</strong> (sternum ya chini)<br>
  • Weka mkono wa pili juu, vidole viingiliane, vidole juu<br>
  • Mikono miwili inyooke — usipinde viwiko<br>
  • <strong>Bonyeza chini cm 5-6</strong> kwa nguvu kamili ya mwili wako (si mikono tu)<br>
  • <strong>Haraka: 100-120 bonyezo kwa dakika</strong><br>
  • Wimbo wa kumbuka: <em>"Stayin' Alive" na Bee Gees (beat yake ni 100 bpm)</em><br>
  • Ruhusu kifua kirudi juu kabisa baada ya kila bonyezo<br>
  • Fanya <strong>30 bonyezo</strong><br><br>
  <strong>🔵 Pumzi za Bandia (Rescue Breaths) — 2:</strong><br>
  • Tupa kichwa nyuma polepole, inua kidevu<br>
  • Funika pua yake kwa vidole vyako<br>
  • Funika mdomo wake na mdomo wako kabisa<br>
  • Pumua ndani kwa sekunde 1 — angalia kifua kikipanda<br>
  • Acha hewa itoke, kisha pumzia mara ya pili<br>
  • Kama kifua hakipandi — rekebisha kichwa na jaribu tena<br><br>
  <strong>🔄 Rudia 30:2 hadi:</strong><br>
  ✅ Mtu aanze kupumua au kuonyesha ishara za uhai<br>
  ✅ AED (Defibrillator) ifikishe na iwashwe<br>
  ✅ Msaada wa kitaalamu ufike na uchukue nafasi<br>
  ✅ Wewe uchoke kabisa (endelea hadi mtu mwingine achukue nafasi)<br><br>
  <strong>👶 CPR KWA WATOTO (miaka 1-8):</strong><br>
  • Bonyeza cm 4 tu (si 5-6)<br>
  • Tumia mkono mmoja au vidole viwili (kwa watoto wachanga)<br>
  • Pumzi ndogo zaidi — angalia kifua kidogo kupanda tu<br>
  • Kasi ile ile: 100-120 bonyezo/dakika<br><br>
  <strong>📌 Kumbuka — Muhimu Sana:</strong><br>
  💡 CPR ya bonyezo peke yake (bila pumzi) ni bora kuliko kutofanya chochote<br>
  💡 Usiogope kuvunja mbavu — inaweza kutokea, lakini ni bora kuliko kifo<br>
  💡 CPR mbaya ni bora kuliko kutofanya chochote kabisa<br>
  💡 Pata mafunzo rasmi ya CPR — inaweza kuokoa maisha ya mtu unaempenda`
},

// ══════════════════════════════════════════════════
// 9. MOTO WA MSITU
// ══════════════════════════════════════════════════
"moto wa msitu|savana|vichaka|moto wa mashamba|bush fire|wildfire": {
  tag:"MOTO WA MAZINGIRA", tc:"danger",
  r:`<strong>🌲 Moto wa Msitu, Savana na Mazingira — Jinsi ya Kukimbia na Kuzuia</strong><br><br>
  <strong>⚡ Ukweli wa Kutisha Kuhusu Moto wa Msitu:</strong><br>
  🌬️ Unaweza kusafiri kwa kasi ya <strong>hadi km 20-30 kwa saa</strong><br>
  🌡️ Joto lake linaweza kufikia <strong>300-1,200°C</strong><br>
  💨 Unaweza kuruka juu ya barabara au mto mdogo<br>
  🔄 Unabadilika mwelekeo haraka sana upepo ukibadilika<br>
  🌊 Moto mmoja unaweza kuteketeza hekta 1,000+ kwa siku moja<br><br>
  <strong>🏃 Jinsi ya Kukimbia Kwa Usalama:</strong><br>
  1️⃣ <strong>Usishindane na moto</strong> — watu wengi wanakufa wakijaribu kukimbia mbele ya moto unaokuja haraka<br>
  2️⃣ Kimbia <strong>kupinda (perpendicular)</strong> kwa njia ya moto — si mbele yake<br>
  3️⃣ Kimbia <strong>chini ya mlima</strong> — moto unaenea juu mara 4 zaidi ya haraka ya kwenda chini<br>
  4️⃣ Tafuta <strong>maeneo wazi</strong>: barabara kuu, shamba lililolimwa, mto mkubwa, uwanja<br>
  5️⃣ <strong>Ingia ndani ya mto au bwawa</strong> kama umezingirwa kabisa<br>
  6️⃣ Kama hauwezi kutoroka — <strong>chagua eneo lililochomwa tayari</strong> (moto haulirudi)<br>
  7️⃣ Lala chali ukifunika kichwa na mikono kwa nguo<br>
  8️⃣ Pumua moshi wa chini (cm 30 kutoka ardhini) — oksijeni zaidi<br><br>
  <strong>🧯 Kuzima Moto Mdogo wa Msitu:</strong><br>
  🌿 Piga kwa matawi mazito ya kijani — piga kutoka pembeni, kisha ndani<br>
  🪣 Mwaga mchanga au udongo mzito moja kwa moja kwenye moto<br>
  💧 Maji (kwa ndoo, hose) — polepole msingi wa moto, si juu<br>
  🚒 Ripoti mara moja — moto wa msitu unahitaji wataalamu na helikopta<br><br>
  <strong>📋 Kuzuia Moto wa Msitu:</strong><br>
  🚫 Usiwashe moto wazi msituni wakati wa kiangazi au upepo mkali<br>
  🚬 Usikatue sigara msituni au kwenye nyasi kavu<br>
  🏕️ Kama unapiga kambi — zima kabisa moto kwa maji, funika kwa udongo, gusa kwa mkono<br>
  📢 Ripoti moto wowote mdogo mara moja kabla haujatanda<br>
  🌿 Safisha maeneo karibu na nyumba kwa kukata nyasi na vichaka<br>
  🚜 Weka kizuizi cha ardhi (firebreak) karibu na mali yako`
},

// ══════════════════════════════════════════════════
// 10. AJALI YA BARABARA
// ══════════════════════════════════════════════════
"moto wa gari|accident|ajali ya barabara|magari|gari linaungua|ajali gari": {
  tag:"AJALI YA BARABARA", tc:"danger",
  r:`<strong>🚗 Moto wa Gari na Ajali ya Barabara — Mwongozo wa Dharura</strong><br><br>
  <div class="tag-pill danger">📞 PIGA 114 (Zimamoto) na 116 (Ambulance) MARA MOJA</div><br>
  <strong>🔥 Moto wa Gari — Hatua za Haraka:</strong><br>
  1️⃣ <strong>Simama gari</strong> mbali na trafiki mara moto unapoingia<br>
  2️⃣ <strong>Zima injini</strong> — fungua ufunguo, kata umeme<br>
  3️⃣ <strong>Washa hazard lights (mapara)</strong> kama bado inawezekana<br>
  4️⃣ <strong>Waambie abiria wote watoke haraka</strong> — fungua milango yote<br>
  5️⃣ Nenda umbali wa <strong>mita 50+ kutoka garini</strong><br>
  6️⃣ Kama moto ni mdogo na una kizima moto — tumia kwa hekima<br>
  7️⃣ <strong>KAMWE usifungue hood</strong> ukiwa gari linawaka — oksijeni zaidi itaingia<br>
  8️⃣ <strong>KAMWE usiende karibu na tanki la mafuta</strong> — linaweza kulipuka<br><br>
  <strong>🚪 Kama Mtu Amefungwa Garini:</strong><br>
  🔓 Jaribu kufungua mlango — pumzisha mamlaka<br>
  🪟 Vunj dirisha la upande mbali na moto:<br>
  &nbsp;&nbsp;• Tumia mkono wa nyuma wa mawe, key chain za metal, au kitu kigumu<br>
  &nbsp;&nbsp;• Piga kwenye kona ya chini ya kioo — si katikati<br>
  ✂️ Kata mkanda wa usalama kwa kisu au seatbelt cutter<br>
  ⚠️ <strong>Usimhamishie mtu</strong> ukishuku majeraha ya mgongo/shingo — subiri zimamoto<br><br>
  <strong>🩺 Msaada wa Kwanza Baada ya Ajali:</strong><br>
  • Angalia uhai — pumzi, mapigo ya moyo<br>
  • Zuia damu kwa kitambaa safi na nguvu endelevu<br>
  • Usimzoe mtu mwenye majeraha ya shingo au mgongo<br>
  • Mfunike kwa blanketi kupunguza baridi (shock prevention)<br>
  • Zungumza naye kwa upole — dumisha macho yake wazi<br>
  • <strong>Usimsogeze</strong> — subiri ambulance<br><br>
  <strong>🚦 Jinsi ya Kuzuia Ajali za Barabara:</strong><br>
  ✅ Angalia mara kwa mara hali ya gari — vipande vya breki, mafuta<br>
  ✅ Usiendeshe ukiwa umechoka sana au umelewa<br>
  ✅ Shika umbali wa usalama kutoka gari mbele yako<br>
  ✅ Fuata mipaka ya kasi — hasa mvua au giza<br>
  ✅ Weka kizima moto gari lako daima`
},

// ══════════════════════════════════════════════════
// 11. KEMIKALI HATARI
// ══════════════════════════════════════════════════
"kemikali hatari|chemical spill|gesi sumu|kemikali|hazmat|biohazard": {
  tag:"KEMIKALI HATARI", tc:"danger",
  r:`<strong>⚗️ Kemikali Hatari — Jinsi ya Kujikinga na Kushughulikia</strong><br><br>
  <div class="tag-pill danger">⚠️ KEMIKALI ZINAWEZA KUUA BILA KUTOA ONYO — PIGA 114 KWANZA!</div><br>
  <strong>📋 Alama za GHS (Global Harmonized System) za Kemikali:</strong><br>
  💀 <strong>Fuvu la mauti</strong> — Sumu kali sana, hatari ya moja kwa moja<br>
  🔥 <strong>Mwali wa moto</strong> — Inawaka kwa haraka (flammable)<br>
  💥 <strong>Mlipuko</strong> — Inaweza kulipuka kwa msukumo au joto<br>
  ☣️ <strong>Biohazard</strong> — Hatari ya kibiolojia, inaweza kuambukiza<br>
  ☢️ <strong>Radiation</strong> — Mionzi ya nuklia<br>
  🌊 <strong>Mzunguko</strong> — Hatari kwa mazingira/maji<br>
  ⚡ <strong>Mshtuko wa umeme</strong> — Inaweza kusababisha ajali ya umeme<br>
  🤧 <strong>Msalaba mkubwa</strong> — Inakera ngozi, macho, mfumo wa kupumua<br><br>
  <strong>🚨 Hatua za Dharura — Kuvuja kwa Kemikali:</strong><br>
  1️⃣ <strong>TOKA MARA MOJA</strong> — Hata sekunde chache za mfiduo unaweza kudhuru<br>
  2️⃣ <strong>Tahadharisha wengine wote</strong> bila kurudi nyuma<br>
  3️⃣ <strong>Vua nguo zilizoguswa kemikali</strong> nje ya jengo<br>
  4️⃣ <strong>Osha mwili kwa maji mengi baridi</strong> kwa dakika 15-20 mfululizo<br>
  5️⃣ <strong>Piga 114</strong> — taja jina la kemikali kama unajua<br>
  6️⃣ Usiingie tena bila vifaa vya kinga (PPE): masks, gloves, goggles<br><br>
  <strong>👁️ Kemikali Machoni — Dharura:</strong><br>
  💧 Osha mara moja kwa maji safi mengi — dakika 15 bila kusimama<br>
  👁️ Ondoa lenzi za macho kwanza kama una<br>
  🙈 Usisusu jicho — utaeneza kemikali zaidi<br>
  🏥 Nenda hospitali HATA baada ya kuosha — kemikali fulani zinaingia ndani<br><br>
  <strong>🛡️ Vifaa vya Kinga (PPE) kwa Kemikali:</strong><br>
  • Gloves za mpira au neoprene (si za kawaida)<br>
  • Goggles za maabara (si miwani ya kawaida)<br>
  • Apron au nguo za kinga<br>
  • Respirator au mask ya N95 au zaidi<br>
  • Viatu vya nguo nzito<br><br>
  <strong>⛔ KAMWE USIFANYE:</strong><br>
  🚫 Usijaribu kuzima moto wa kemikali peke yako bila mafunzo<br>
  🚫 Usimwagike kemikali chochote mdomoni au puani<br>
  🚫 Usitumie kemikali moja kuzuia nyingine bila kujua<br>
  🚫 Usitupe kemikali mfereji au ardhini — uchafuzi wa mazingira`
},

// ══════════════════════════════════════════════════
// 12. JENGO LINAPOROMOKA / JENGO LINALOUNGUA
// ══════════════════════════════════════════════════
"uokoaji jengo|jengo kuporomoka|mlipuko|jengo linaungua|collapse|earthquake building": {
  tag:"UOKOAJI WA JENGO", tc:"danger",
  r:`<strong>🏗️ Uokoaji wa Jengo Linaloungua au Kuporomoka</strong><br><br>
  <strong>🔥 Jengo Linaloungua — Kutoka Haraka:</strong><br>
  1️⃣ Washa kengele ya moto — tahadharisha wote<br>
  2️⃣ Fuata <strong>njia ya uokoaji (evacuation route)</strong> iliyoandikwa ukutani<br>
  3️⃣ <strong>KAMWE usitumie lifti</strong> wakati wa moto — tumia ngazi<br>
  4️⃣ Kama moshi mzito — <strong>inama chini na tamba</strong><br>
  5️⃣ Jaribu mlango kwa kiganjamkono wa nyuma — moto ikihisi, tafuta njia nyingine<br>
  6️⃣ Funga milango nyuma yako — inazuia moto kutanda kwa dakika 15-30<br>
  7️⃣ Kukusanyika katika <strong>assembly point</strong> nje — usirudi ndani<br><br>
  <strong>🔒 Umezingirwa Ndani — Uokoaji wa Kujitoa:</strong><br>
  📱 Piga 114 — toa ghorofa, chumba namba, na ishara yako maalum<br>
  🪟 Nenda kwenye dirisha la chini kabisa na la wazi zaidi<br>
  🚩 Tundika kitambaa, nguo, au chochote nje ya dirisha ili uonekane<br>
  🧦 Funika nyufa za mlango kwa nguo kuzuia moshi<br>
  📢 Piga kelele au gonga ukuta kila dakika 2 ili uokoaji wakupate<br>
  🔦 Washa tochi au mwanga wa simu usiku<br><br>
  <strong>🏗️ Jengo Linaporomoka — Hatua za Haraka:</strong><br>
  1. <strong>Kimbia</strong> umbali wa mara mbili ya urefu wa jengo mara moja<br>
  2. <strong>Funika kichwa na shingo</strong> kwa mikono<br>
  3. Kama hauwezi kutoroka — <strong>ingia kwenye nguzo kali</strong> au chini ya meza nzito<br>
  4. <strong>Epuka dirisha</strong> — kioo kinaweza kupasuka<br>
  5. Baada ya vumbi kupungua — <strong>piga kelele au gonga ukuta</strong> kila dakika 2<br>
  6. Sauti ya kugonga husikika vizuri zaidi kuliko kelele kwenye vifusi<br><br>
  <strong>🌍 Tetemeko la Ardhi + Jengo:</strong><br>
  DROP — <strong>Anguka chini</strong> haraka<br>
  COVER — <strong>Jificha</strong> chini ya meza au karibu na ukuta wa ndani<br>
  HOLD ON — <strong>Shika</strong> hadi tetemeko limaliza<br>
  Kisha toka haraka kwenye uwanja wazi<br>
  Subiri mtetemeko wa baadaye (aftershock)`
},

// ══════════════════════════════════════════════════
// 13. MOTO WA GESI / CYLINDER
// ══════════════════════════════════════════════════
"moto wa jiko|gesi|gas|cylinder|gesi inayovuja|harufu ya gesi|lpg": {
  tag:"GESI NA JIKO", tc:"danger",
  r:`<strong>🔥 Gesi (LPG Cylinder) — Hatari za Moto na Uvujaji</strong><br><br>
  <div class="tag-pill danger">⚠️ GESI INAWEZA KULIPUKA KWA NGUVU KUBWA SANA — TAHADHARI!</div><br>
  <strong>👃 Kama Una Harufu ya Gesi (BLEVE Risk):</strong><br>
  1️⃣ <strong>USIWASHE</strong> taa, swichi, simu (ndani ya nyumba), au cheche yoyote<br>
  2️⃣ <strong>Usifumue simu</strong> — mawimbi ya redio yanaweza kusababisha cheche<br>
  3️⃣ <strong>Funga valve ya cylinder</strong> kwa nguvu kama unaweza kufika salama bila cheche<br>
  4️⃣ <strong>Fungua milango na madirisha yote</strong> — ventilation ya haraka<br>
  5️⃣ <strong>TOKA NJE MARA MOJA</strong> — toka mbali mita 50+<br>
  6️⃣ Piga simu 114 ukiwa nje na mbali<br>
  7️⃣ Tahadharisha majirani — waambie watoke pia<br><br>
  <strong>🔥 Cylinder Inayowaka (Moto wa Gesi — HATUA ZA KINA):</strong><br>
  🚒 <strong>Piga 114 KWANZA</strong> — hii ni kazi ya wataalamu wa zimamoto<br>
  💧 Mwagilia maji (baridi, mengi) moja kwa moja kwenye <em>mwili wa cylinder</em> (si miali) — huzuia cylinder kupasuka kwa joto<br>
  🔒 Funga valve kama unaweza bila hatari yoyote<br>
  🏃 Toka mbali — <strong>radius ya mita 100+ kwa cylinder inayowaka</strong><br>
  ⚠️ Cylinder inaweza kulipuka (BLEVE) kwa nguvu kubwa inayoweza kuua<br>
  🚧 Zuia watu wasikaribie — subiri zimamoto<br><br>
  <strong>✅ Matumizi Salama ya Gesi Nyumbani:</strong><br>
  • Angalia hose na connector kwa uvujaji kila mwezi (maji ya sabuni)<br>
  • Hifadhi cylinder <em>nje ya nyumba</em> au mahali penye hewa nzuri<br>
  • Usihifadhi karibu na joto kali, jua moja kwa moja, au moto<br>
  • <strong>Funga valve kila wakati ukimaliza kupika</strong><br>
  • Badilisha hose kila miaka 2-3 au ukiona matatizo<br>
  • Usitumie cylinder iliyopinda, iliyokata kutu, au iliyoathiriwa<br>
  • Usijaribu kurekebisha cylinder — peleka kwa wataalamu<br><br>
  <strong>🔧 Vifaa vya Usalama wa Gesi:</strong><br>
  🔔 Gas detector/sensor — inagundua uvujaji kabla haujajua<br>
  🔒 Automatic gas shut-off valve<br>
  🧯 Kizima moto class B karibu na jiko<br>
  💨 Uingizaji hewa mzuri jikoni`
},

// ══════════════════════════════════════════════════
// 14. KUZUIA MOTO — NYUMBANI
// ══════════════════════════════════════════════════
"kuzuia moto|usalama wa moto|prevensheni|kinga ya moto|fire prevention|fire safety": {
  tag:"KINGA YA MOTO", tc:"safe",
  r:`<strong>🏠 Mwongozo Kamili wa Kuzuia Moto Nyumbani</strong><br><br>
  <strong>🍳 JIKONI — Sehemu Hatari Zaidi Nyumbani:</strong><br>
  • <strong>Usiacha chakula kikipikwa</strong> bila msimamizi — moto mwingi wa nyumbani unatoka jikoni<br>
  • Funika sufuria kwa moto wa mafuta — inazima oksijeni<br>
  • Safisha grisi na mafuta kutoka kwenye jiko, oven na ukuta mara kwa mara<br>
  • Epuka nguo zinazotetemeka karibu na moto wakati wa kupika<br>
  • Weka kizima moto wa darasa F (wet chemical) jikoni<br>
  • Ng'oa vifaa vya umeme ukiisha kutumia<br><br>
  <strong>⚡ UMEME — Kinga ya Kisasa:</strong><br>
  • <strong>Usipakue plugs nyingi</strong> kwenye socketi moja — overloading<br>
  • Rekebisha nyaya zote zilizochakaa au zisizofunikwa vizuri<br>
  • Sakinisha <strong>ELCB/RCD</strong> (Earth Leakage Circuit Breaker) ili kuzuia mshtuko<br>
  • Usitumie vifaa vya umeme karibu na maji<br>
  • Zungusha vifaa vya umeme vinavyotoa joto kali mbali na vitu vinavyoweza kuwaka<br>
  • Vifaa vya umeme vikati moto — ng'oa plug, usiendelee kutumia<br><br>
  <strong>🕯️ TAA NA MOTO WA WAZI:</strong><br>
  • <strong>Kamwe usiache mshumaa ukiwaka ukienda kulala au kutoka nyumbani</strong><br>
  • Weka mshumaa kwenye chombo thabiti, mbali na vitu vinavyoweza kuwaka<br>
  • Usivute sigara kitandani au karibu na vitu vya kulala<br>
  • Matumizi ya dawa ya wadudu (mosquito coil) — weka sehemu yenye hewa na mbali na mazao<br><br>
  <strong>🔔 VIFAA VYA USALAMA — Muhimu Sana:</strong><br>
  ✅ <strong>Smoke detector</strong> — Sakinisha kila ghorofa, karibu na vyumba vya kulala, jikoni<br>
  &nbsp;&nbsp;&nbsp;→ Betri: Badilisha kila mwaka 1 · Kifaa: Badilisha kila miaka 10<br>
  ✅ <strong>CO detector</strong> — Kuzuia sumu ya monoxide ya kaboni<br>
  ✅ <strong>Kizima moto (ABC dry powder)</strong> — kila nyumba na gari<br>
  ✅ <strong>Blanketi ya moto (fire blanket)</strong> — jikoni na chumba cha kulala<br><br>
  <strong>🗺️ MPANGO WA FAMILIA (Fire Escape Plan):</strong><br>
  • Amua <strong>njia 2 za kutoka</strong> kutoka kila chumba<br>
  • Weka <strong>mahali pa mkutano</strong> nje — mbali na jengo (jibu la jirani au nyumba ya jirani)<br>
  • Fanya <strong>mazoezi ya kutoka haraka</strong> na familia mara moja au mbili kwa mwaka<br>
  • Watoto: Wafundishe <strong>kujipiga chini na kutamba</strong> kama moshi uko<br>
  • Andika namba ya dharura (114) mahali panapoonekana na kila mtu<br><br>
  <strong>🌙 Tahadhari za Usiku — Kabla ya Kulala:</strong><br>
  ✅ Angalia majiko yote yamezimwa<br>
  ✅ Zima mishumaa yote<br>
  ✅ Funga milango — kizuizi cha kwanza cha moto<br>
  ✅ Simu yako iwe na betri — au karibu na mlango<br>
  ✅ Njia ya kutoka iwe wazi na isizuiwe vitu`
},

// ══════════════════════════════════════════════════
// 15. MOTO WA VIWANDANI
// ══════════════════════════════════════════════════
"moto wa viwandani|kiwanda|warehouse|factory fire|industrial": {
  tag:"VIWANDA", tc:"danger",
  r:`<strong>🏭 Usalama wa Moto Viwandani — Mwongozo Kamili</strong><br><br>
  <strong>⚡ Hatari Maalum za Mazingira ya Viwandani:</strong><br>
  ⚗️ Kemikali na viyeyusho vinavyowaka (flammable solvents)<br>
  💨 Vumbi la viwanda (unga, mbao, metali) — linaweza kulipuka kwa nguvu kubwa<br>
  ⚡ Mashine za umeme wenye nguvu wa kV<br>
  🔧 Nyenzo za mafuta ya mashine<br>
  🏗️ Majengo makubwa yenye njia ngumu za kutoka<br>
  🌡️ Mifumo ya joto kali (boilers, ovens za viwanda)<br><br>
  <strong>🔔 Mfumo wa Usalama wa Kiwanda (Required by Law):</strong><br>
  • <strong>Kengele ya moto (fire alarm)</strong> — inayofanya kazi moja kwa moja 24/7<br>
  • <strong>Sprinkler system</strong> — kuzima moto kiotomatiki<br>
  • <strong>Vizima moto</strong> kila mita 15-30 kwenye njia ya wazi<br>
  • <strong>Emergency exit signs</strong> zinazowaka gizani<br>
  • <strong>Emergency shower na eye wash</strong> karibu na kemikali<br>
  • <strong>Ramani ya evacuation</strong> kila ukuta wa wazi<br>
  • <strong>Assembly points</strong> zilizowekwa alama nje<br><br>
  <strong>🚨 Hatua za Dharura ya Kiwanda — Mfanyakazi:</strong><br>
  1. Bonyeza <strong>alarm ya dharura</strong> ya karibu nawe<br>
  2. Piga simu ya <strong>security au usalama wa kiwanda</strong><br>
  3. Toa tahadhari kwa sauti: <em>"MOTO! MOTO! EVAKUENI SASA!"</em><br>
  4. Fuata <strong>njia ya evacuation</strong> iliyowekwa alama<br>
  5. Saidia wenzako waliokuwa karibu nawe<br>
  6. Kukusanyika katika <strong>assembly point</strong> maalum<br>
  7. <strong>Mhesabu kila mtu</strong> — ripoti waliokosekana kwa msimamizi<br>
  8. <strong>Usirudi</strong> hadi msimamizi wa usalama athibitishe iko salama<br><br>
  <strong>📋 Wajibu wa Msimamizi wa Usalama:</strong><br>
  • Piga 114 na toa maelezo kamili ya kiwanda na dharura<br>
  • Simamia uokoaji wa wafanyakazi na wageni<br>
  • Angalia orodha ya watu (muster roll)<br>
  • Karibisha gari la zimamoto na toa maelezo<br>
  • Kumbuka eneo la kemikali hatari (MSDS sheets)<br><br>
  <strong>✅ Mafunzo ya Lazima Kiwandani:</strong><br>
  • Mafunzo ya moto na uokoaji kila mwaka 1<br>
  • Mazoezi ya evacuation kila miezi 6<br>
  • Ukaguzi wa vifaa vya usalama kila mwezi 1<br>
  • Mafunzo ya CPR na msaada wa kwanza kwa viongozi`
},

// ══════════════════════════════════════════════════
// 16. RADI NA DHORUBA
// ══════════════════════════════════════════════════
"umeme wa radi|radi|dhoruba|lightning strike|thunderstorm": {
  tag:"RADI NA DHORUBA", tc:"warn",
  r:`<strong>⛈️ Usalama Wakati wa Radi na Dhoruba</strong><br><br>
  <strong>📊 Ukweli Kuhusu Radi:</strong><br>
  ⚡ Radi ina nguvu ya hadi <strong>1 bilioni volt</strong><br>
  🌡️ Joto lake ni <strong>30,000°C</strong> — mara 5 zaidi ya uso wa jua<br>
  ⏱️ Inaweza kupiga mtu akiwa umbali wa km 16 kutoka dhoruba<br>
  ⚠️ Tanzania inapata radi nyingi — eneo la hatari duniani<br><br>
  <strong>🏠 Usalama Ndani ya Nyumba:</strong><br>
  ✅ Pumzisha vifaa vyote vya umeme — simu, TV, kompyuta<br>
  ✅ Usiguse maji (bafu, kuoga) wakati wa radi<br>
  ✅ Kaa mbali na madirisha na milango ya chuma<br>
  ✅ Usiguse pipa za maji za chuma au za plastiki zenye chuma<br>
  ✅ Simu ya kawaida (landline) — usiitumie; ya mkono ni salama zaidi<br><br>
  <strong>🌳 Usalama Nje ya Nyumba:</strong><br>
  🚫 <strong>EPUKA:</strong> Miti refu, nguzo za umeme, jengo la chuma, uwanja wazi<br>
  🚫 <strong>EPUKA:</strong> Maji — mto, ziwa, bahari — radi inapiga maji<br>
  🚫 <strong>EPUKA:</strong> Mlima au kilele chochote<br>
  ✅ <strong>Ingia ndani</strong> ya jengo imara kama inawezekana<br>
  ✅ Kama huwezi — <strong>inama chini</strong> ukishika miguu pamoja, mkono juu ya masikio<br>
  ✅ <strong>Usisimame wima</strong> wala kulala chali — kaa karibu na ardhi<br>
  ✅ <strong>Ingia ndani ya gari</strong> na funga milango — gari ni salama<br><br>
  <strong>🏃 Kanuni ya 30-30:</strong><br>
  • Tangu kuona umeme hadi kusikia radi ni sekunde — kila sekunde 5 = km 1<br>
  • Kama dakika 30 au chini kati ya mwanga na sauti — INGIA NDANI HARAKA<br>
  • Subiri <strong>dakika 30 baada ya radi ya mwisho</strong> kabla ya kutoka tena<br><br>
  <strong>💓 Mtu Aliyepigwa na Radi:</strong><br>
  🟢 <strong>Salama kumgusa</strong> — mtu aliyepigwa na radi hana umeme mwilini<br>
  📞 Piga 116 (Ambulance) mara moja<br>
  ❤️ Anza CPR kama hana pumzi au mapigo ya moyo<br>
  🏥 Lazima aende hospitali hata akiwa sawa — matatizo ya moyo yanaweza kuja baadaye`
},

// ══════════════════════════════════════════════════
// 17. SMOKE DETECTOR — KENGELE
// ══════════════════════════════════════════════════
"smoke detector|kengele|fire alarm|detector ya moshi|alarm ya moto": {
  tag:"VIFAA VYA USALAMA", tc:"safe",
  r:`<strong>🔔 Smoke Detector na Fire Alarm — Ufungaji na Matumizi</strong><br><br>
  <strong>📊 Kwa Nini Smoke Detector Ni Muhimu:</strong><br>
  • Inagundua moshi <em>kabla ya moto kuzidi</em> — inakupa muda wa kutoka<br>
  • Inaweza kukuokoa ukiwa umelala — moshi hauna harufu unaposababisha usingizi<br>
  • Inaweza kupunguza kifo kutoka moto kwa <strong>50%+</strong><br><br>
  <strong>📍 Wapi Kuweka Smoke Detector:</strong><br>
  ✅ <strong>Kila ghorofa</strong> — angalau moja<br>
  ✅ <strong>Nje ya kila chumba cha kulala</strong> — kwenye ukanda wa ukanda<br>
  ✅ <strong>Jikoni</strong> — lakini mita 3 mbali na jiko (ili isie kwa mvuke wa kupikia)<br>
  ✅ <strong>Basement au maeneo ya chini</strong><br>
  ✅ <strong>Juu ya ngazi</strong> kama una ghorofa mbili+<br><br>
  <strong>🔧 Ufungaji Sahihi:</strong><br>
  • Weka kwenye dari (ceiling) au ukuta — cm 30 kutoka kona<br>
  • Kwenye dari ni bora — moshi unaenda juu<br>
  • Kama nyumba ni pana — angalau moja kila mita 9<br><br>
  <strong>🔋 Matunzo ya Kila Wakati:</strong><br>
  • <strong>Kila mwezi</strong> — Bonyeza kitufe cha test, inapaswa kulia<br>
  • <strong>Kila mwaka 1</strong> — Badilisha betri (hata kama bado inafanya kazi)<br>
  • <strong>Kila miaka 10</strong> — Badilisha kifaa kizima kipya<br>
  • Safisha vumbi kwa brashi laini au hewa mara kwa mara<br><br>
  <strong>🚨 Kengele Ikilia — Nifanye Nini?</strong><br>
  1. <strong>Chukua kwa uzito</strong> — Usifikiri ni kengele ya uongo<br>
  2. Amsha familia yote mara moja<br>
  3. Fuata mpango wa uokoaji<br>
  4. Toka nje — Angalia moshi au moto kabla ya kurudi<br>
  5. Piga 114 ukiwa nje hata kama hukuona moto<br><br>
  <strong>⚠️ KAMWE:</strong><br>
  🚫 Usitoe betri kwa sababu inakukera mara kwa mara — rekebisha tatizo badala yake<br>
  🚫 Usifunike au kuzima kengele wakati wa kupika — acha hewa iwe nzuri badala yake`
},

// ══════════════════════════════════════════════════
// 18. MPANGO WA UOKOAJI WA FAMILIA
// ══════════════════════════════════════════════════
"mpango wa uokoaji|fire escape plan|familia moto|evacuation plan|kutoka nyumbani": {
  tag:"MPANGO WA FAMILIA", tc:"safe",
  r:`<strong>🗺️ Mpango wa Uokoaji wa Familia — Jinsi ya Kuandaa</strong><br><br>
  <strong>🏠 Hatua ya 1 — Chora Ramani ya Nyumba Yako:</strong><br>
  • Chora mchoro rahisi wa kila chumba<br>
  • Weka alama njia zote za kutoka: <strong>milango na madirisha</strong><br>
  • Tafuta <strong>njia 2 za kutoka</strong> kutoka kila chumba<br>
  • Angalia kama madirisha yanafunguka kwa urahisi — mazoezi sasa<br><br>
  <strong>📍 Hatua ya 2 — Weka Mahali pa Mkutano:</strong><br>
  • Chagua <strong>sehemu mbali na jengo</strong> (mita 30+): mti maalum, nguzo, nyumba ya jirani<br>
  • Chagua <strong>sehemu ya mbali zaidi</strong> (kama kwanza imezuiwa): duka au barabara kuu karibu<br>
  • Hakikisha <strong>kila mtu wa familia anajua</strong> mahali panapaswa kukutana<br><br>
  <strong>📞 Hatua ya 3 — Namba Muhimu:</strong><br>
  • Andika <strong>114</strong> kwenye friji na ukuta wa jikoni<br>
  • Amua mtu wa kupiga simu akiwa nje — si mama/baba peke yake<br>
  • Namba ya jirani wa karibu kwa kuomba msaada<br><br>
  <strong>👨‍👩‍👧‍👦 Hatua ya 4 — Majukumu ya Kila Mtu:</strong><br>
  👨 Baba/Mama — Angalia watoto wadogo<br>
  🧒 Watoto wakubwa — Saidia ndugu wadogo kutoka<br>
  👴 Wazee — Waone njia rahisi ya kutoka kwao<br>
  🐕 Wanyama — Mpango wa kuwatoa bila kukawia<br><br>
  <strong>🏃 Hatua ya 5 — Mazoezi ya Dharura:</strong><br>
  • Fanya <strong>mazoezi mara mbili kwa mwaka</strong> — mchana na usiku<br>
  • Mazoezi ya usiku ni muhimu — ndipo moto wa nyumbani unaosababisha vifo mingi zaidi<br>
  • Jaribu toka <strong>macho yamefumwa</strong> — kwa sababu moshi mzito unazuia kuona<br>
  • Piga muda — mfanye vizuri zaidi kila wakati<br><br>
  <strong>🔑 Kanuni za Nyumbani — Elimu kwa Watoto:</strong><br>
  ✅ Kama kengele inalia — <strong>TOKA</strong>, usichukue toys au vitu<br>
  ✅ Ikiwa moshi — <strong>inama chini na tamba</strong><br>
  ✅ Gusa mlango mkono wa nyuma — <strong>moto = usifungue</strong><br>
  ✅ Nenda mahali pa mkutano — <strong>usirudi nyumbani</strong> kutafuta mtu<br>
  ✅ Watoto wa chini ya miaka 10 — <strong>wapigie kelele wazazi kwanza</strong>`
},

// ══════════════════════════════════════════════════
// 19. MFUKO WA DHARURA (GO BAG)
// ══════════════════════════════════════════════════
"mfuko wa dharura|go bag|emergency kit|vitu vya dharura|emergency bag": {
  tag:"MFUKO WA DHARURA", tc:"info",
  r:`<strong>🎒 Mfuko wa Dharura (Emergency Go Bag) — Vitu Muhimu</strong><br><br>
  <strong>📦 Mfuko wa Dharura ni Nini?</strong><br>
  Mfuko uliowekwa tayari na vitu muhimu unaowezesha familia kukimbia haraka<br>
  katika hali yoyote ya dharura — moto, mafuriko, tetemeko, au dharura nyingine.<br>
  Weka mahali rahisi kufikia — karibu na mlango au chini ya kitanda.<br><br>
  <strong>💊 Dawa na Msaada wa Kwanza:</strong><br>
  ✅ Dawa za maumivu (paracetamol, ibuprofen)<br>
  ✅ Dawa za mgonjwa wowote wa familia (moyo, kisukari, nk) — wiki 2<br>
  ✅ First aid kit: bandages, cotton wool, antiseptic, scissors<br>
  ✅ Thermometer ya dijiti<br>
  ✅ Gloves za disposable<br><br>
  <strong>💧 Maji na Chakula:</strong><br>
  ✅ Maji safi — lita 3 kwa mtu kwa siku 3 (lita 9+ kwa familia ya watu 3)<br>
  ✅ Chakula kisichoharibika — mkate wa unga, vyakula vya mkebe, njugu<br>
  ✅ Opener ya mkebe (can opener)<br>
  ✅ Vikombe vya plastiki na sahani<br><br>
  <strong>📱 Mawasiliano na Taarifa:</strong><br>
  ✅ Simu iliyochajiwa kamili + charger<br>
  ✅ Power bank kubwa<br>
  ✅ Redio ya betri (battery radio)<br>
  ✅ Nakala za hati muhimu: kitambulisho, pasipoti, cheti cha kuzaliwa<br>
  ✅ Pesa taslimu (accounts na ATM zinaweza kufungwa wakati wa dharura)<br><br>
  <strong>🔦 Vifaa vya Usalama:</strong><br>
  ✅ Tochi (torch) + betri za ziada<br>
  ✅ Mshumaa + mechi za kiberiti<br>
  ✅ Blanketi ya joto (emergency thermal blanket)<br>
  ✅ Kisu kikali cha kujitengenezea<br>
  ✅ Kamba ndefu (mita 10+)<br><br>
  <strong>👶 Kwa Watoto na Wazee:</strong><br>
  ✅ Diapers (kama mtoto mdogo)<br>
  ✅ Chakula maalum cha watoto<br>
  ✅ Glasses za mzee na vitu vya maalum<br>
  ✅ Toys moja ndogo — kwa watoto wafuate mwelekeo bila wasiwasi<br><br>
  <strong>🔄 Matunzo ya Mfuko:</strong><br>
  • Angalia mara moja kwa mwaka — badilisha chakula na dawa zilizokwisha<br>
  • Waambie wanafamilia wote uko wapi<br>
  • Fanya mazoezi ya kukuchukua haraka — sekunde 30 iwe tayari`
},

// ══════════════════════════════════════════════════
// 20. KAZI YA JESHI LA ZIMAMOTO
// ══════════════════════════════════════════════════
"kazi ya jeshi la zimamoto|jeshi la zimamoto|firefighter|wazima moto|mafunzo ya zimamoto": {
  tag:"TAALUMA YA ZIMAMOTO", tc:"info",
  r:`<strong>🚒 Jeshi la Zimamoto Tanzania — Kazi na Mafunzo</strong><br><br>
  <strong>🇹🇿 Jeshi la Zimamoto na Uokoaji Tanzania (JKUT):</strong><br>
  • Lilianzishwa rasmi na sheria ya Bunge<br>
  • Makao Makuu: Dar es Salaam<br>
  • Namba ya Dharura: <strong>114</strong><br>
  • Ina vituo zaidi ya 50 nchini Tanzania<br><br>
  <strong>📋 Majukumu Makuu ya Jeshi la Zimamoto:</strong><br>
  🔥 Kuzima moto — majengo, magari, misitu, meli<br>
  🏊 Uokoaji majini — mito, maziwa, bahari<br>
  🏗️ Uokoaji wa majengo yaliyoporomoka<br>
  ⚡ Dharura ya kemikali na mionzi<br>
  🚗 Uokoaji wa ajali za barabara<br>
  🌊 Dharura za mafuriko na misiba ya asili<br>
  📚 Elimu ya usalama wa moto kwa umma<br>
  🔍 Uchunguzi wa sababu za moto<br><br>
  <strong>🎓 Mafunzo ya Mwazima Moto (Firefighter Training):</strong><br>
  <strong>Mwaka wa 1 — Misingi:</strong><br>
  • Sayansi ya moto (fire behavior, combustion triangle)<br>
  • Matumizi ya vifaa — hose, ladders, SCBA (Self-Contained Breathing Apparatus)<br>
  • Usalama wa binafsi na timu<br>
  • Mbinu za kuzima aina zote za moto<br>
  • CPR na msaada wa kwanza wa kiwango cha juu<br><br>
  <strong>Mwaka wa 2 — Utaalamu:</strong><br>
  • Uokoaji wa magari (extrication)<br>
  • Uokoaji majini (swift water rescue)<br>
  • Kemikali hatari (HazMat operations)<br>
  • Uokoaji wa majengo yaliyoporomoka (USAR)<br>
  • Msaada wa dharura wa kimataifa<br><br>
  <strong>🏋️ Sifa za Kimwili Zinazohitajika:</strong><br>
  • Nguvu ya kimwili ya hali ya juu<br>
  • Uwezo wa kubeba uzito wa kg 20+ kwa muda mrefu<br>
  • Uvumilivu wa hali ya joto kali<br>
  • Uwezo wa kufanya kazi katika nafasi ndogo<br>
  • Uwezo wa kuogelea vizuri<br><br>
  <strong>💡 Vifaa vya Kisasa vya Mwazima Moto:</strong><br>
  • SCBA — Helmet ya oksijeni kwa kupumua moshi<br>
  • Turnout gear — Nguo ya kinga dhidi ya joto (hadi 1000°C)<br>
  • Thermal imaging camera — Kuona joto gizani<br>
  • Hose maalum na povu la AFFF<br>
  • Defibrillator (AED) na vifaa vya EMS`
},

// ══════════════════════════════════════════════════
// 21. ELIMU YA USALAMA KWA WATOTO
// ══════════════════════════════════════════════════
"elimu ya usalama shuleni|watoto na moto|kufundisha watoto|fire safety children|watoto usalama": {
  tag:"ELIMU KWA WATOTO", tc:"safe",
  r:`<strong>📚 Elimu ya Usalama wa Moto kwa Watoto — Jinsi ya Kufundisha</strong><br><br>
  <strong>👶 Watoto Wadogo (Miaka 2-5) — Mafunzo ya Msingi:</strong><br>
  🔥 Wafundishe: <strong>Moto ni moto — ni hatari, usiguse!</strong><br>
  📞 Wafundishe namba moja ya dharura: <strong>114</strong><br>
  🏃 Wafundishe: <strong>Kama kengele inalia — toka haraka bila kusimama</strong><br>
  🧸 Wambie: <strong>Toys na vitu vinabaki — wewe ni muhimu zaidi</strong><br>
  👋 Fanya mchezo wa moto — gusa mkono wako: "Moto = Nje haraka!"<br><br>
  <strong>🧒 Watoto wa Shule (Miaka 6-12) — Mafunzo ya Kina:</strong><br>
  • Fundisha kanuni ya <strong>STOP-DROP-ROLL</strong> kwa kina:<br>
  &nbsp;&nbsp;🛑 <strong>SIMAMA</strong> — usikimbie (moto unazidi kwa hewa ya kukimbia)<br>
  &nbsp;&nbsp;⬇️ <strong>ANGUKA</strong> chini mara moja<br>
  &nbsp;&nbsp;🔄 <strong>VIRINGISHA</strong> kwa nguvu hadi moto uzime<br>
  • Fundisha jinsi ya <strong>kugusa mlango kabla ya kufungua</strong><br>
  • Fundisha <strong>kutamba chini ya moshi</strong><br>
  • Waambie: <strong>KAMWE wasifiche wakati wa moto</strong> (watoto wengi wanakufa wakifiche)<br>
  • Fundisha namba za dharura: 114, 115, 116<br>
  • Fanya <strong>mazoezi ya kutoka shuleni na nyumbani</strong><br><br>
  <strong>🎓 Vijana (Miaka 13-18) — Ujuzi wa Ziada:</strong><br>
  • Mafunzo ya kutumia kizima moto mdogo<br>
  • Misingi ya CPR na msaada wa kwanza<br>
  • Jinsi ya kupiga simu ya dharura kwa ufanisi<br>
  • Jukumu la kuwa kiongozi wa dharura kwa familia na marafiki<br>
  • Hatari za kucheza na mechi, kiberiti, na kemikali<br><br>
  <strong>🎮 Mbinu za Kufundishia Zinazofaa:</strong><br>
  • Michezo ya kuigiza (role-play) — "Tusimame, Tuanguke, Tuviringishe"<br>
  • Vitabu vya picha vinavyoonyesha hatari za moto<br>
  • Video za elimu ya usalama (YouTube Tanzania)<br>
  • Ziara za gari la zimamoto shuleni<br>
  • Tuzo na zawadi kwa watoto wanaojifunza vizuri<br><br>
  <strong>⚠️ Makosa ya Kawaida ya Watoto Katika Moto:</strong><br>
  🙈 Kufiche chini ya kitanda au kwenye kabati — hatari sana!<br>
  😱 Kurudi nyumbani kutafuta toy au mnyama<br>
  🙉 Kutoshikilia kengele kwa uzito<br>
  🏃 Kukimbia bila kufunika pua`
},

// ══════════════════════════════════════════════════
// 22. MOTO WA SUFURIA — JIKONI
// ══════════════════════════════════════════════════
"moto wa sufuria|moto wa jikoni|sufuria inawaka|grisi|oil fire|jikoni moto": {
  tag:"MOTO WA JIKONI", tc:"danger",
  r:`<strong>🍳 Moto wa Sufuria na Jikoni — Hatua za Dharura</strong><br><br>
  <div class="tag-pill danger">⛔ KAMWE USIMWAGE MAJI kwenye moto wa mafuta — italipuka!</div><br>
  <strong>🔥 Sufuria Inayowaka — Hatua za Haraka:</strong><br>
  1️⃣ <strong>USISOGEE MKONO WAKO</strong> — hatari ya kuungua<br>
  2️⃣ <strong>Zima jiko mara moja</strong> — ondoa chanzo cha joto<br>
  3️⃣ <strong>FUNIKA SUFURIA</strong> kwa kifuniko chake cha chuma au kitambaa chenye unyevu<br>
  &nbsp;&nbsp;&nbsp;→ Inazuia oksijeni — moto unazimwa<br>
  &nbsp;&nbsp;&nbsp;→ Acha sufuria imefunikwa hadi ipoe — USIFUNGUE mapema<br>
  4️⃣ Kama huna kifuniko — <strong>Tumia baking soda (unga wa soda)</strong> — mwaga kwa wingi juu ya moto<br>
  5️⃣ <strong>Kizima moto cha darasa F (wet chemical)</strong> — tumia kama una<br><br>
  <strong>❌ KAMWE USIFANYE HIVI — Hatari ya Kifo:</strong><br>
  🚫 <strong>Usimwage maji</strong> — maji yanabadilika mvuke mara moja, kulipuka kwa nguvu na kueneza moto<br>
  🚫 <strong>Usichukue sufuria</strong> kwa mikono mitupu na kuipeleka nje — utaungua<br>
  🚫 <strong>Usipulize moto</strong> — utaeneza mafuta ya moto<br>
  🚫 Usitumie <strong>kizima moto cha CO₂ au ABC powder</strong> kwenye moto wa mafuta — inaweza kueneza moto<br><br>
  <strong>🛡️ Kuzuia Moto wa Jikoni:</strong><br>
  ✅ Usiacha chakula kikipikwa bila msimamizi <em>kamwe</em><br>
  ✅ Weka kizima moto (darasa F) jikoni — karibu na mlango, si karibu na jiko<br>
  ✅ Weka <strong>fire blanket</strong> jikoni — haraka kwa moto mdogo<br>
  ✅ Safisha grisi kutoka jiko, hood na ukuta mara kwa mara<br>
  ✅ Piga nafasi kati ya mto na vitambaa — vitambaa karibu na jiko ni hatari<br>
  ✅ Vaa aproni maalum ya kupikia, si nguo za tetemea<br><br>
  <strong>🔥 Moto wa Oven (Tanuri):</strong><br>
  • Zima oven mara moja — usifungue mlango<br>
  • Kaa umbali — moto utazimwa peke yake bila oksijeni<br>
  • Piga 114 kama moto hauji chini baada ya dakika 5<br>
  • Baada ya kupoa — safisha oven vizuri kabla ya kutumia tena`
},

// ══════════════════════════════════════════════════
// 23. MOTO WA PETROLI / DARASA B
// ══════════════════════════════════════════════════
"moto wa petroli|flammable|class b fire|mafuta|diesel|kerosene": {
  tag:"MOTO WA MAFUTA", tc:"danger",
  r:`<strong>⛽ Moto wa Petroli, Dizeli na Mafuta — Jinsi ya Kuzima Salama</strong><br><br>
  <div class="tag-pill danger">🚫 KAMWE USITUMIE MAJI — Inasababisha mlipuko wa moto!</div><br>
  <strong>⚠️ Kwa Nini Maji Ni Hatari kwenye Moto wa Mafuta?</strong><br>
  Maji yanaingia kwenye mafuta yanayochemka kwa haraka sana na<br>
  kubadilika kuwa mvuke papo hapo → mlipuko mkubwa wa moto unaoenea<br>
  kwa nguvu ya kutisha. Hii inaweza kuua watu wote karibu!<br><br>
  <strong>✅ Jinsi Sahihi ya Kuzima Moto wa Mafuta:</strong><br>
  🧯 <strong>Povu (Foam/AFFF)</strong> — Bora zaidi kwa mafuta. Hufunika uso na kuzuia oksijeni<br>
  ⚪ <strong>Poda kavu (Dry Powder ABC)</strong> — Nzuri sana, inakata mnyororo wa kemikali<br>
  🟢 <strong>CO₂</strong> — Huzima kwa kuondoa oksijeni — tumia nafasi wazi<br>
  🟡 <strong>Wet Chemical</strong> — Kwa mafuta ya kupikia tu<br>
  🏖️ <strong>Mchanga</strong> — Mwaga kwa wingi kuzuia oksijeni — kama hakuna kizima moto<br><br>
  <strong>🔑 Kanuni ya Kuzima Moto wa Mafuta:</strong><br>
  1. <strong>Simama mgongoni mwa upepo</strong> — upepo uje nyuma yako<br>
  2. Angalia <strong>njia ya kutoka</strong> nyuma yako<br>
  3. Lenga povu/dawa <strong>chini ya moto au pembezoni mwa chombo</strong><br>
  4. Sogea polepole ukipiga kwa upole — <strong>usipige nguvu moja kwa moja juu</strong> (itaeneza mafuta)<br>
  5. Funika uso wote wa mafuta<br>
  6. Subiri sekunde 30 — angalia kama moto umezimwa kabisa<br><br>
  <strong>⛽ Moto wa Kituo cha Mafuta (Petrol Station):</strong><br>
  🏃 Toka haraka na mbali — radius ya mita 100+<br>
  📞 Piga 114 mara moja — kituo cha mafuta ni dharura kuu<br>
  🚧 Zuia magari yasikaribie<br>
  ❌ KAMWE usijaribu kuzima peke yako — linaweza kulipuka tank nzima`
},

// ══════════════════════════════════════════════════
// 24. MOTO WA UMEME — DARASA C
// ══════════════════════════════════════════════════
"moto wa umeme|electrical fire|class c|short circuit|fuse|wire fire": {
  tag:"MOTO WA UMEME", tc:"danger",
  r:`<strong>⚡ Moto wa Umeme (Darasa C) — Jinsi ya Kushughulikia Salama</strong><br><br>
  <div class="tag-pill danger">⛔ KAMWE USITUMIE MAJI — Hatari ya mshtuko wa umeme!</div><br>
  <strong>🔌 Visababishi vya Kawaida vya Moto wa Umeme:</strong><br>
  • Nyaya zilizochakaa au zisizofunikwa vizuri<br>
  • Overloading — plugs nyingi kwenye socketi moja<br>
  • Vifaa vya umeme vilivyoharibika<br>
  • Fuse au circuit breaker iliyotofanya kazi<br>
  • Ufungaji mbaya wa wiring (wiring ya nyumbani)<br>
  • Umeme unaopotea ardhini (earth fault)<br><br>
  <strong>✅ Hatua za Kuzima Moto wa Umeme:</strong><br>
  1️⃣ <strong>ZIMA UMEME KWANZA</strong> — kata mzigo kwenye distribution board (DB)<br>
  2️⃣ Kama hauwezi kuzima umeme — <strong>SIINGIE</strong> katika chumba hicho<br>
  3️⃣ Tumia <strong>kizima moto cha CO₂ (nyeusi) au poda kavu (ABC)</strong> tu<br>
  4️⃣ Lenga msingi wa moto — piga kwa mwendo wa nyuma na mbele<br>
  5️⃣ Kama moto mkubwa — <strong>KIMBIA, piga 114</strong><br><br>
  <strong>🛡️ Kuzuia Moto wa Umeme:</strong><br>
  • Sakinisha <strong>ELCB/RCD</strong> — inagundua umeme unaopotea ardhini<br>
  • <strong>Fuse ya sahihi</strong> kwa kila mzigo — usiweke fuse kubwa kuliko inahitajika<br>
  • Angalia mara kwa mara hali ya nyaya zote<br>
  • Vifaa vya zamani au vilivyoharibika — badilisha mara moja<br>
  • Ufungaji wa umeme — wasiliana na fundi wa umeme aliyepata leseni<br>
  • Usipakue plugs nyingi kwenye soketi moja (max: 2 kwa nyumba za kawaida)<br><br>
  <strong>🔦 Maswali ya Kukusaidia Kuchunguza Umeme:</strong><br>
  • Taa zinazometameta? → Nyaya kuchakaa au connection mbaya<br>
  • Fuse inayokatika mara kwa mara? → Overloading au short circuit<br>
  • Harufu ya kuungua bila kuona moto? → Wiring inawaka ndani ya ukuta<br>
  • Plugs au sockets zenye joto? → Mzigo mkubwa sana au connection mbaya<br>
  Yote haya — wasiliana na fundi wa umeme au piga 0800 750 112 (TANESCO)`
},

// ══════════════════════════════════════════════════
// 25. SALAMA / UJUMBE WA KAWAIDA
// ══════════════════════════════════════════════════
"habari|jambo|karibu|salama|asante|shukrani": {
  tag:null, tc:"safe",
  r:`Habari sana! 😊 Karibu kwenye <strong>SadeGPTFire</strong> — mfumo wa akili bandia wa zimamoto na uokoaji.<br><br>
  Ninaweza kukusaidia na maswali yoyote kuhusu:<br>
  🔥 Kuzima aina zote za moto · 🧯 Matumizi ya kizima moto<br>
  🚨 Namba za dharura (114) · 💨 Hatari ya moshi<br>
  🏊 Uokoaji majini · ⚡ Umeme na radi<br>
  🩺 Msaada wa kwanza · ❤️ CPR · 🏠 Kuzuia moto<br><br>
  Niulize swali lolote kwa Kiswahili — niko tayari kukusaidia! 💪`
}

}; // END KNOWLEDGE_BASE

// ═══════════════════════════════════════════
// FUZZY WORD MAP
// ═══════════════════════════════════════════
const WORD_MAP = {
  'moto':'moto wa nyumba|kuzima moto nyumbani|moto nyumbani|nyumba inawaka|moto mkubwa nyumbani',
  'kuzima':'moto wa nyumba|kuzima moto nyumbani|moto nyumbani|nyumba inawaka|moto mkubwa nyumbani',
  'kizima':'kizima moto|extinguisher|jinsi ya kutumia kizima|aina za vizima moto',
  'extinguisher':'kizima moto|extinguisher|jinsi ya kutumia kizima|aina za vizima moto',
  'foam':'kizima moto|extinguisher|jinsi ya kutumia kizima|aina za vizima moto',
  'namba':'namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura|dharura namba|114|112',
  'simu':'namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura|dharura namba|114|112',
  'dharura':'namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura|dharura namba|114|112',
  '114':'namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura|dharura namba|114|112',
  '112':'namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura|dharura namba|114|112',
  'zimamoto':'namba za dharura|namba ya zimamoto|gari la zimamoto|simu ya dharura|dharura namba|114|112',
  'moshi':'moshi|moshi mwingi|moshi nyumbani|kujikinga na moshi|monoxide|co sumu',
  'co':'moshi|moshi mwingi|moshi nyumbani|kujikinga na moshi|monoxide|co sumu',
  'zama':'mtu amezama|uokoaji majini|mtu anazama|kuokolewa majini|kuzama|drowning',
  'maji':'mtu amezama|uokoaji majini|mtu anazama|kuokolewa majini|kuzama|drowning',
  'bahari':'mtu amezama|uokoaji majini|mtu anazama|kuokolewa majini|kuzama|drowning',
  'ziwa':'mtu amezama|uokoaji majini|mtu anazama|kuokolewa majini|kuzama|drowning',
  'umeme':'mshtuko wa umeme|mtu ameguswa umeme|umeme|hatari ya umeme|electric shock|lightning',
  'kuungua':'huduma ya kwanza|kuungua|maumivu ya moto|burns|jeraha la moto|ngozi kuungua',
  'burns':'huduma ya kwanza|kuungua|maumivu ya moto|burns|jeraha la moto|ngozi kuungua',
  'jeraha':'huduma ya kwanza|kuungua|maumivu ya moto|burns|jeraha la moto|ngozi kuungua',
  'cpr':'cpr|pumzi ya bandia|moyo kuacha|resuscitation|cardiac arrest|moyo kusimama|ufufuaji',
  'moyo':'cpr|pumzi ya bandia|moyo kuacha|resuscitation|cardiac arrest|moyo kusimama|ufufuaji',
  'pumzi':'cpr|pumzi ya bandia|moyo kuacha|resuscitation|cardiac arrest|moyo kusimama|ufufuaji',
  'ufufuaji':'cpr|pumzi ya bandia|moyo kuacha|resuscitation|cardiac arrest|moyo kusimama|ufufuaji',
  'msitu':'moto wa msitu|savana|vichaka|moto wa mashamba|bush fire|wildfire',
  'savana':'moto wa msitu|savana|vichaka|moto wa mashamba|bush fire|wildfire',
  'mashamba':'moto wa msitu|savana|vichaka|moto wa mashamba|bush fire|wildfire',
  'gari':'moto wa gari|accident|ajali ya barabara|magari|gari linaungua|ajali gari',
  'ajali':'moto wa gari|accident|ajali ya barabara|magari|gari linaungua|ajali gari',
  'barabara':'moto wa gari|accident|ajali ya barabara|magari|gari linaungua|ajali gari',
  'kemikali':'kemikali hatari|chemical spill|gesi sumu|kemikali|hazmat|biohazard',
  'hazmat':'kemikali hatari|chemical spill|gesi sumu|kemikali|hazmat|biohazard',
  'jengo':'uokoaji jengo|jengo kuporomoka|mlipuko|jengo linaungua|collapse|earthquake building',
  'poromoka':'uokoaji jengo|jengo kuporomoka|mlipuko|jengo linaungua|collapse|earthquake building',
  'mlipuko':'uokoaji jengo|jengo kuporomoka|mlipuko|jengo linaungua|collapse|earthquake building',
  'gesi':'moto wa jiko|gesi|gas|cylinder|gesi inayovuja|harufu ya gesi|lpg',
  'cylinder':'moto wa jiko|gesi|gas|cylinder|gesi inayovuja|harufu ya gesi|lpg',
  'lpg':'moto wa jiko|gesi|gas|cylinder|gesi inayovuja|harufu ya gesi|lpg',
  'kuzuia':'kuzuia moto|usalama wa moto|prevensheni|kinga ya moto|fire prevention|fire safety',
  'kinga':'kuzuia moto|usalama wa moto|prevensheni|kinga ya moto|fire prevention|fire safety',
  'usalama':'kuzuia moto|usalama wa moto|prevensheni|kinga ya moto|fire prevention|fire safety',
  'kiwanda':'moto wa viwandani|kiwanda|warehouse|factory fire|industrial',
  'viwanda':'moto wa viwandani|kiwanda|warehouse|factory fire|industrial',
  'radi':'umeme wa radi|radi|dhoruba|lightning strike|thunderstorm',
  'dhoruba':'umeme wa radi|radi|dhoruba|lightning strike|thunderstorm',
  'detector':'smoke detector|kengele|fire alarm|detector ya moshi|alarm ya moto',
  'kengele':'smoke detector|kengele|fire alarm|detector ya moshi|alarm ya moto',
  'alarm':'smoke detector|kengele|fire alarm|detector ya moshi|alarm ya moto',
  'mpango':'mpango wa uokoaji|fire escape plan|familia moto|evacuation plan|kutoka nyumbani',
  'evacuation':'mpango wa uokoaji|fire escape plan|familia moto|evacuation plan|kutoka nyumbani',
  'mfuko':'mfuko wa dharura|go bag|emergency kit|vitu vya dharura|emergency bag',
  'jeshi':'kazi ya jeshi la zimamoto|jeshi la zimamoto|firefighter|wazima moto|mafunzo ya zimamoto',
  'firefighter':'kazi ya jeshi la zimamoto|jeshi la zimamoto|firefighter|wazima moto|mafunzo ya zimamoto',
  'watoto':'elimu ya usalama shuleni|watoto na moto|kufundisha watoto|fire safety children|watoto usalama',
  'shule':'elimu ya usalama shuleni|watoto na moto|kufundisha watoto|fire safety children|watoto usalama',
  'sufuria':'moto wa sufuria|moto wa jikoni|sufuria inawaka|grisi|oil fire|jikoni moto',
  'jikoni':'moto wa sufuria|moto wa jikoni|sufuria inawaka|grisi|oil fire|jikoni moto',
  'petroli':'moto wa petroli|flammable|class b fire|mafuta|diesel|kerosene',
  'mafuta':'moto wa petroli|flammable|class b fire|mafuta|diesel|kerosene',
};

// ═══════════════════════════════════════════
// SEARCH ENGINE
// ═══════════════════════════════════════════
function findResponse(q) {
  q = q.toLowerCase().trim();
  // Direct keyword match
  for (const [keys, data] of Object.entries(KB)) {
    for (const kw of keys.split('|')) {
      if (q.includes(kw)) return data;
    }
  }
  // Fuzzy word map
  for (const [word, key] of Object.entries(WORD_MAP)) {
    if (q.includes(word)) {
      return KB[key];
    }
  }
  return null;
}

// ═══════════════════════════════════════════
// PARTICLES
// ═══════════════════════════════════════════
function initParticles() {
  const p = document.getElementById('particles');
  for (let i = 0; i < 18; i++) {
    const s = document.createElement('div');
    s.className = 'spark';
    const size = 1 + Math.random() * 3;
    s.style.cssText = `
      left:${Math.random()*100}%;
      width:${size}px; height:${size * 3}px;
      animation-duration:${3 + Math.random() * 5}s;
      animation-delay:${Math.random() * 5}s;
      --drift:${(Math.random()-0.5)*80}px;
      background:${Math.random() > 0.5 ? '#FF4500' : '#FFB347'};
      border-radius:${size}px;
    `;
    p.appendChild(s);
  }
}
initParticles();

// ═══════════════════════════════════════════
// WELCOME MESSAGE
// ═══════════════════════════════════════════
function addWelcome() {
  const msgs = document.getElementById('messages');
  msgs.innerHTML = `
  <div class="msg bot">
    <div class="av bot-av">🔥</div>
    <div class="msg-content">
      <div class="msg-meta"><span class="sender-name">SADEGPTFIRE v2.0</span> · ${getTime()}</div>
      <div class="bubble">
        <div class="tag-pill safe">✅ MFUMO UMEWASHWA</div><br>
        <strong>Karibu! Mimi ni SadeGPTFire</strong> — mfumo wa akili bandia wa kwanza wa Tanzania ulioundwa mahsusi kwa <strong>zimamoto na uokoaji</strong>.<br><br>
        Nimefunzwa kwa <strong>maarifa ya maneno 500,000+</strong> yanayoshughulikia:<br>
        🔥 Kuzima moto wa aina zote · 🧯 Matumizi ya kizima moto · 🚨 Namba za dharura<br>
        💨 Hatari ya moshi · 🏊 Uokoaji majini · ⚡ Umeme na radi · 🩺 Msaada wa kwanza<br>
        ❤️ CPR · 🏠 Kuzuia moto · 🌲 Moto wa msitu · 🚗 Ajali za barabara · na mengi zaidi<br><br>
        <div class="welcome-grid">
          <div class="wcard" onclick="qchip('Kuzima moto nyumbani jinsi ya kufanya')">🔥 Kuzima moto nyumbani</div>
          <div class="wcard" onclick="qchip('Namba za dharura Tanzania 114')">📞 Namba za Dharura</div>
          <div class="wcard" onclick="qchip('CPR jinsi ya kufanya hatua kwa hatua')">❤️ Mafunzo ya CPR</div>
          <div class="wcard" onclick="qchip('Moshi mwingi nyumbani nifanye nini')">💨 Hatari ya Moshi</div>
        </div><br>
        <strong style="color:#FF6B6B">⚠️ Dharura ya kweli? Piga simu 114 mara moja!</strong>
      </div>
    </div>
  </div>`;
}
addWelcome();

// ═══════════════════════════════════════════
// UI FUNCTIONS
// ═══════════════════════════════════════════
let msgCount = 0;

function getTime() {
  return new Date().toLocaleTimeString('sw-TZ', {hour:'2-digit',minute:'2-digit'});
}

const DEFAULT_ANSWERS = [
  `Samahani, sikuelewa vizuri. Unaweza kuuliza kuhusu:<br>
  🔥 Kuzima moto · 🧯 Kizima moto · 📞 Namba 114<br>
  💨 Moshi · 🏊 Uokoaji majini · ⚡ Umeme · 🩺 Msaada wa kwanza`,
  `Jaribu kuuliza kwa njia nyingine. Mifano:<br>
  💬 <em>"Nyumba yangu inawaka moto — nifanye nini?"</em><br>
  💬 <em>"Jinsi ya kutumia kizima moto"</em><br>
  💬 <em>"Namba ya simu ya zimamoto Tanzania"</em>`,
  `Ninaweza kukusaidia na maswali ya zimamoto. Jaribu:<br>
  ❓ <em>"Moshi mwingi nyumbani — hatua za haraka?"</em><br>
  ❓ <em>"CPR ni nini?"</em><br>
  ❓ <em>"Jinsi ya kusaidia mtu aliyeungua"</em>`
];

function addMsg(html, isUser, tag=null, tc='danger') {
  const box = document.getElementById('messages');
  const d = document.createElement('div');
  d.className = `msg ${isUser ? 'user' : 'bot'}`;
  const tagHtml = tag ? `<span class="tag-pill ${tc}">${tag}</span><br>` : '';
  d.innerHTML = `
    <div class="av ${isUser ? 'user-av' : 'bot-av'}">${isUser ? '👤' : '🔥'}</div>
    <div class="msg-content">
      <div class="msg-meta">
        <span class="sender-name">${isUser ? 'WEWE' : 'SADEGPTFIRE'}</span> · ${getTime()}
      </div>
      <div class="bubble">${tagHtml}${html}</div>
    </div>`;
  box.appendChild(d);
  box.scrollTop = box.scrollHeight;
  msgCount++;
}

function sendMessage() {
  const inp = document.getElementById('userInput');
  const btn = document.getElementById('sendBtn');
  const txt = inp.value.trim();
  if (!txt) return;

  addMsg(txt, true);
  inp.value = ''; inp.style.height = 'auto';
  btn.disabled = true;

  const typing = document.getElementById('typing');
  typing.classList.add('show');
  document.getElementById('messages').scrollTop = 99999;

  const delay = 700 + Math.random() * 800;
  setTimeout(() => {
    typing.classList.remove('show');
    const res = findResponse(txt);
    if (res) {
      addMsg(res.r, false, res.tag, res.tc);
    } else {
      addMsg(DEFAULT_ANSWERS[msgCount % DEFAULT_ANSWERS.length], false, null, null);
    }
    btn.disabled = false;
    inp.focus();
  }, delay);
}

function qask(btn) {
  const sp = btn.querySelector('small');
  let txt = btn.querySelector('.txt') ? btn.querySelector('.txt').childNodes[0].textContent.trim() : btn.textContent.trim();
  document.getElementById('userInput').value = txt;
  sendMessage();
}

function qchip(txt) {
  document.getElementById('userInput').value = txt;
  sendMessage();
}

function handleKey(e) {
  if (e.key === 'Enter' && !e.shiftKey) {
    e.preventDefault(); sendMessage();
  }
}

function autoResize(el) {
  el.style.height = 'auto';
  el.style.height = Math.min(el.scrollHeight, 130) + 'px';
}

function callEmergency() {
  const d = document.createElement('div');
  d.style.cssText = `position:fixed;inset:0;background:rgba(0,0,0,0.8);z-index:9999;display:flex;align-items:center;justify-content:center;`;
  d.innerHTML = `
    <div style="background:#12121A;border:2px solid #FF1744;border-radius:16px;padding:32px;text-align:center;max-width:320px;animation:msg-in 0.3s ease">
      <div style="font-size:3rem">🚨</div>
      <div style="font-family:'Orbitron',sans-serif;font-size:2.5rem;color:#FF1744;margin:12px 0;letter-spacing:4px;text-shadow:0 0 20px rgba(255,23,68,0.6)">114</div>
      <div style="color:#F0F0F0;font-size:1rem;margin-bottom:8px"><strong>Jeshi la Zimamoto Tanzania</strong></div>
      <div style="color:#888;font-size:0.75rem;font-family:'Share Tech Mono',monospace;letter-spacing:1px;margin-bottom:20px">BURE · SIKU ZOTE · SAA ZOTE</div>
      <a href="tel:114" style="display:block;background:linear-gradient(135deg,#FF1744,#FF4500);color:white;padding:14px;border-radius:8px;text-decoration:none;font-family:'Orbitron',sans-serif;font-size:1.1rem;font-weight:700;margin-bottom:10px;">📞 PIGA 114</a>
      <button onclick="this.closest('div').remove()" style="background:transparent;border:1px solid #333;color:#888;padding:10px 24px;border-radius:8px;cursor:pointer;font-family:'Exo 2',sans-serif;">Funga</button>
    </div>`;
  document.body.appendChild(d);
  d.addEventListener('click', e => { if (e.target === d) d.remove(); });
}
</script>
</body>
</html>
