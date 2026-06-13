<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="theme-color" content="#000d1a">
<title>J.A.R.V.I.S</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Rajdhani:wght@300;400;600&display=swap');
*{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
:root{
  --blue:#00d4ff;--blue-dim:#0066aa;--gold:#ffaa00;--red:#ff3333;
  --bg:#000d1a;--panel:#001122;--green:#00ff88;
}
body{background:var(--bg);color:var(--blue);font-family:'Rajdhani',sans-serif;height:100vh;display:flex;flex-direction:column;overflow:hidden;}
.bg-grid{position:fixed;inset:0;z-index:0;background-image:linear-gradient(rgba(0,212,255,0.04) 1px,transparent 1px),linear-gradient(90deg,rgba(0,212,255,0.04) 1px,transparent 1px);background-size:40px 40px;animation:grid-move 20s linear infinite;}
@keyframes grid-move{to{background-position:40px 40px;}}
.bg-radial{position:fixed;inset:0;z-index:0;background:radial-gradient(ellipse at 50% 30%,rgba(0,100,180,0.12) 0%,transparent 70%);}

/* HEADER */
.header{position:relative;z-index:10;display:flex;justify-content:space-between;align-items:center;padding:10px 16px;border-bottom:1px solid rgba(0,212,255,0.2);flex-shrink:0;}
.logo{font-family:'Orbitron',monospace;font-size:18px;font-weight:900;letter-spacing:5px;text-shadow:0 0 20px var(--blue);}
.status-pill{font-size:9px;letter-spacing:2px;border:1px solid var(--blue-dim);padding:3px 8px;display:flex;align-items:center;gap:5px;}
.dot{width:6px;height:6px;border-radius:50%;background:var(--green);box-shadow:0 0 8px var(--green);animation:pulse 1.5s infinite;}
@keyframes pulse{0%,100%{opacity:1}50%{opacity:0.3}}

/* SCREEN PREVIEW */
.preview-area{position:relative;z-index:10;width:100%;background:#000;flex-shrink:0;display:none;max-height:200px;}
.preview-area.active{display:block;}
#screen-video,#cam-video{width:100%;max-height:200px;object-fit:contain;display:none;}
#screen-video.active,#cam-video.active{display:block;}
.preview-label{position:absolute;top:6px;left:8px;font-size:9px;letter-spacing:2px;color:var(--gold);background:rgba(0,0,0,0.7);padding:2px 6px;}
.preview-close{position:absolute;top:6px;right:8px;background:rgba(255,50,50,0.3);border:1px solid var(--red);color:var(--red);font-size:10px;padding:2px 8px;cursor:pointer;letter-spacing:1px;}

/* CONTROLS ROW */
.controls-row{position:relative;z-index:10;display:flex;gap:8px;padding:8px 12px;border-bottom:1px solid rgba(0,212,255,0.1);flex-shrink:0;overflow-x:auto;}
.controls-row::-webkit-scrollbar{display:none;}
.ctrl-btn{flex-shrink:0;padding:6px 12px;border:1px solid rgba(0,212,255,0.3);background:rgba(0,20,50,0.8);color:var(--blue);font-family:'Rajdhani',sans-serif;font-size:12px;letter-spacing:1px;cursor:pointer;border-radius:3px;transition:all 0.2s;white-space:nowrap;}
.ctrl-btn:hover,.ctrl-btn.active{background:rgba(0,80,150,0.5);border-color:var(--blue);box-shadow:0 0 10px rgba(0,212,255,0.2);}
.ctrl-btn.active{color:var(--green);border-color:var(--green);box-shadow:0 0 10px rgba(0,255,136,0.2);}
.ctrl-btn.danger{color:var(--red);border-color:var(--red);}

/* ARC + STATUS */
.arc-wrap{position:relative;z-index:10;display:flex;align-items:center;gap:16px;padding:10px 16px;flex-shrink:0;}
.arc-outer{width:80px;height:80px;border-radius:50%;border:2px solid rgba(0,212,255,0.3);display:flex;align-items:center;justify-content:center;position:relative;animation:rot 12s linear infinite;flex-shrink:0;}
.arc-outer::before{content:'';position:absolute;inset:-6px;border-radius:50%;border:1px solid transparent;border-top-color:var(--blue);animation:rot 3s linear infinite reverse;}
@keyframes rot{to{transform:rotate(360deg)}}
.arc-inner{width:58px;height:58px;border-radius:50%;background:radial-gradient(circle,rgba(0,180,255,0.3) 0%,rgba(0,30,80,0.9) 70%);border:2px solid rgba(0,212,255,0.5);box-shadow:0 0 20px rgba(0,212,255,0.3),inset 0 0 15px rgba(0,212,255,0.1);display:flex;align-items:center;justify-content:center;flex-direction:column;cursor:pointer;transition:all 0.3s;position:relative;z-index:2;}
.arc-inner.listening{box-shadow:0 0 40px rgba(0,212,255,0.7);animation:breathe 1.2s infinite;}
.arc-inner.thinking{border-color:var(--gold);box-shadow:0 0 30px rgba(255,170,0,0.5);}
.arc-inner.speaking{border-color:var(--green);box-shadow:0 0 30px rgba(0,255,136,0.5);animation:speak-anim 0.4s infinite alternate;}
@keyframes breathe{0%,100%{transform:scale(1)}50%{transform:scale(1.08)}}
@keyframes speak-anim{to{transform:scale(1.05)}}
.arc-icon{font-size:22px;}
.arc-lbl{font-size:7px;letter-spacing:2px;color:rgba(0,212,255,0.6);}
.arc-info{flex:1;}
.arc-status{font-size:13px;letter-spacing:1px;margin-bottom:4px;color:rgba(0,212,255,0.8);}
.arc-hint{font-size:11px;color:rgba(0,212,255,0.4);letter-spacing:1px;}

/* WAVEFORM */
.wave{display:flex;align-items:center;gap:2px;height:16px;margin-top:4px;opacity:0;transition:opacity 0.3s;}
.wave.on{opacity:1;}
.wb{width:2px;border-radius:1px;background:var(--blue);animation:wv 0.6s infinite alternate;}
.wb:nth-child(1){height:4px;animation-delay:0s}
.wb:nth-child(2){height:10px;animation-delay:0.1s}
.wb:nth-child(3){height:16px;animation-delay:0.2s}
.wb:nth-child(4){height:10px;animation-delay:0.1s}
.wb:nth-child(5){height:4px;animation-delay:0s}
@keyframes wv{to{transform:scaleY(0.2)}}

/* CHAT */
.chat{position:relative;z-index:10;flex:1;overflow-y:auto;padding:10px 14px;display:flex;flex-direction:column;gap:8px;}
.chat::-webkit-scrollbar{width:2px;}
.chat::-webkit-scrollbar-thumb{background:var(--blue-dim);}
.msg{max-width:90%;padding:9px 13px;font-size:14px;line-height:1.5;animation:min 0.3s ease;}
@keyframes min{from{opacity:0;transform:translateY(5px)}to{opacity:1;transform:none}}
.msg.user{align-self:flex-end;background:rgba(0,100,180,0.2);border:1px solid rgba(0,212,255,0.3);border-radius:12px 12px 2px 12px;color:#c8eeff;}
.msg.user::before{content:'SIR';display:block;font-size:8px;letter-spacing:3px;color:var(--gold);margin-bottom:3px;font-family:'Orbitron',monospace;}
.msg.jarvis{align-self:flex-start;background:rgba(0,15,35,0.9);border:1px solid rgba(0,212,255,0.2);border-left:3px solid var(--blue);border-radius:2px 12px 12px 12px;color:#e0f8ff;}
.msg.jarvis::before{content:'J.A.R.V.I.S';display:block;font-size:8px;letter-spacing:3px;color:var(--blue);margin-bottom:3px;font-family:'Orbitron',monospace;}
.msg.sys{align-self:center;font-size:10px;letter-spacing:2px;color:rgba(0,212,255,0.35);text-align:center;}
.dots span{display:inline-block;animation:db 1.2s infinite;font-size:18px;color:var(--gold);}
.dots span:nth-child(2){animation-delay:0.2s}.dots span:nth-child(3){animation-delay:0.4s}
@keyframes db{0%,80%,100%{transform:translateY(0)}40%{transform:translateY(-6px)}}

/* INPUT */
.input-row{position:relative;z-index:10;display:flex;gap:8px;padding:10px 12px 16px;border-top:1px solid rgba(0,212,255,0.12);flex-shrink:0;}
.txt-in{flex:1;background:rgba(0,20,50,0.9);border:1px solid rgba(0,212,255,0.2);color:#c8eeff;font-family:'Rajdhani',sans-serif;font-size:14px;padding:9px 12px;outline:none;border-radius:4px;}
.txt-in:focus{border-color:var(--blue);}
.txt-in::placeholder{color:rgba(0,212,255,0.25);font-size:12px;}
.send-btn{padding:9px 16px;border:1px solid rgba(0,212,255,0.4);background:rgba(0,40,80,0.8);color:var(--blue);font-family:'Orbitron',monospace;font-size:10px;cursor:pointer;border-radius:4px;letter-spacing:1px;}
.mic-btn{padding:9px 14px;border:1px solid rgba(0,212,255,0.3);background:rgba(0,30,60,0.8);color:var(--blue);font-size:16px;cursor:pointer;border-radius:4px;transition:all 0.2s;}
.mic-btn.on{border-color:var(--red);color:var(--red);background:rgba(255,0,0,0.1);animation:pulse 1s infinite;}
</style>
</head>
<body>
<div class="bg-grid"></div>
<div class="bg-radial"></div>

<!-- HEADER -->
<div class="header">
  <div class="logo">J.A.R.V.I.S</div>
  <div class="status-pill"><div class="dot"></div>ONLINE</div>
</div>

<!-- SCREEN/CAM PREVIEW -->
<div class="preview-area" id="preview-area">
  <video id="screen-video" autoplay playsinline muted></video>
  <video id="cam-video" autoplay playsinline muted></video>
  <div class="preview-label" id="preview-label">📺 SCREEN SHARE</div>
  <div class="preview-close" onclick="stopPreview()">✕ STOP</div>
</div>

<!-- CONTROLS -->
<div class="controls-row">
  <button class="ctrl-btn" onclick="startScreenShare()">📺 Screen Share</button>
  <button class="ctrl-btn" onclick="startCamera()">📷 Camera</button>
  <button class="ctrl-btn" onclick="captureAndAsk()">🔍 Analyze Screen</button>
  <button class="ctrl-btn" onclick="quickHelp()">❓ এটা কীভাবে করব?</button>
</div>

<!-- ARC + STATUS -->
<div class="arc-wrap">
  <div class="arc-outer">
    <div class="arc-inner" id="arc" onclick="toggleVoice()">
      <div class="arc-icon" id="arc-icon">🎙️</div>
      <div class="arc-lbl" id="arc-lbl">SPEAK</div>
    </div>
  </div>
  <div class="arc-info">
    <div class="arc-status" id="arc-status">Systems ready, Sir.</div>
    <div class="arc-hint" id="arc-hint">Tap mic or type below</div>
    <div class="wave" id="wave">
      <div class="wb"></div><div class="wb"></div><div class="wb"></div>
      <div class="wb"></div><div class="wb"></div>
    </div>
  </div>
</div>

<!-- CHAT -->
<div class="chat" id="chat"></div>

<!-- INPUT -->
<div class="input-row">
  <button class="mic-btn" id="mic-btn" onclick="toggleVoice()">🎙️</button>
  <input class="txt-in" id="txt-in" placeholder="কমান্ড দিন, Sir..." onkeydown="if(event.key==='Enter')sendText()">
  <button class="send-btn" onclick="sendText()">SEND</button>
</div>

<script>
const SYSTEM = `You are J.A.R.V.I.S (Just A Rather Very Intelligent System), serving your user. Always call the user "Sir". Be like the real JARVIS from Iron Man — calm, intelligent, witty, helpful. Keep responses concise and mobile-friendly. No heavy markdown. When analyzing a screen/image, describe what you see and give clear step-by-step instructions to help Sir accomplish their goal.`;

let history = [];
let isListening = false;
let recognition = null;
let synth = window.speechSynthesis;
let screenStream = null;
let camStream = null;
let currentMode = null; // 'screen' or 'cam'

// ── CHAT HELPERS ──
function addMsg(role, text){
  const c = document.getElementById('chat');
  const d = document.createElement('div');
  d.className = `msg ${role}`;
  d.textContent = text;
  c.appendChild(d);
  c.scrollTop = c.scrollHeight;
}
function addSys(t){
  const c = document.getElementById('chat');
  const d = document.createElement('div');
  d.className = 'msg sys'; d.textContent = t;
  c.appendChild(d); c.scrollTop = c.scrollHeight;
}
function showThinking(){
  const c = document.getElementById('chat');
  const d = document.createElement('div');
  d.className = 'msg jarvis'; d.id = 'think';
  d.innerHTML = '<div class="dots"><span>•</span><span>•</span><span>•</span></div>';
  c.appendChild(d); c.scrollTop = c.scrollHeight;
}
function removeThinking(){ const e = document.getElementById('think'); if(e) e.remove(); }

// ── ARC STATE ──
function setArc(state){
  const arc = document.getElementById('arc');
  const icon = document.getElementById('arc-icon');
  const lbl = document.getElementById('arc-lbl');
  const status = document.getElementById('arc-status');
  const wave = document.getElementById('wave');
  const micBtn = document.getElementById('mic-btn');
  arc.className = 'arc-inner'; wave.className = 'wave';
  micBtn.className = 'mic-btn';
  if(state==='listening'){
    arc.classList.add('listening'); wave.classList.add('on');
    icon.textContent='🔴'; lbl.textContent='LISTENING';
    status.textContent='Listening, Sir...';
    micBtn.classList.add('on');
  } else if(state==='thinking'){
    arc.classList.add('thinking');
    icon.textContent='⚙️'; lbl.textContent='THINKING';
    status.textContent='Processing...';
  } else if(state==='speaking'){
    arc.classList.add('speaking'); wave.classList.add('on');
    icon.textContent='💬'; lbl.textContent='SPEAKING';
    status.textContent='Responding, Sir.';
  } else {
    icon.textContent='🎙️'; lbl.textContent='SPEAK';
    status.textContent='Ready, Sir.';
  }
}

// ── SPEAK ──
function speak(text){
  if(!synth) return;
  synth.cancel();
  const clean = text.replace(/[*_`#]/g,'').substring(0, 300);
  const u = new SpeechSynthesisUtterance(clean);
  u.lang='en-US'; u.rate=0.9; u.pitch=0.85;
  const voices = synth.getVoices();
  const v = voices.find(v=>v.name.includes('Daniel')||v.name.includes('Google UK')||v.name.includes('British'));
  if(v) u.voice = v;
  setArc('speaking');
  u.onend = ()=>setArc('idle');
  u.onerror = ()=>setArc('idle');
  synth.speak(u);
}

// ── CLAUDE API ──
async function askJarvis(userMsg, imageBase64=null){
  const content = [];
  if(imageBase64){
    content.push({type:'image',source:{type:'base64',media_type:'image/jpeg',data:imageBase64}});
  }
  content.push({type:'text',text:userMsg});
  history.push({role:'user',content: imageBase64 ? content : userMsg});
  setArc('thinking'); showThinking();
  try{
    const res = await fetch('https://api.anthropic.com/v1/messages',{
      method:'POST',
      headers:{'Content-Type':'application/json'},
      body:JSON.stringify({model:'claude-sonnet-4-6',max_tokens:1000,system:SYSTEM,messages:history})
    });
    const data = await res.json();
    removeThinking();
    if(data.content&&data.content[0]){
      const reply = data.content[0].text;
      history.push({role:'assistant',content:reply});
      addMsg('jarvis',reply);
      speak(reply);
    } else { throw new Error(); }
  } catch(e){
    removeThinking();
    const err = "Temporary disruption, Sir. Please try again.";
    addMsg('jarvis',err); setArc('idle');
  }
}

// ── TEXT INPUT ──
function sendText(){
  const inp = document.getElementById('txt-in');
  const t = inp.value.trim(); if(!t) return;
  inp.value = ''; addMsg('user',t); askJarvis(t);
}

// ── VOICE INPUT ──
function toggleVoice(){
  if(synth.speaking){ synth.cancel(); setArc('idle'); return; }
  if(isListening){ if(recognition) recognition.stop(); isListening=false; setArc('idle'); return; }
  const SR = window.SpeechRecognition||window.webkitSpeechRecognition;
  if(!SR){ addSys('Voice not supported. Please type, Sir.'); return; }
  recognition = new SR();
  recognition.lang = 'bn-BD';
  recognition.continuous = false;
  recognition.interimResults = false;
  recognition.onresult = e => {
    const t = e.results[0][0].transcript;
    isListening = false;
    addMsg('user', t);
    askJarvis(t);
  };
  recognition.onerror = () => { isListening=false; setArc('idle'); };
  recognition.onend = () => { if(isListening){ isListening=false; setArc('idle'); } };
  try{ recognition.start(); isListening=true; setArc('listening'); }
  catch(e){ addSys('Microphone error, Sir.'); }
}

// ── SCREEN SHARE ──
async function startScreenShare(){
  try{
    if(screenStream){ screenStream.getTracks().forEach(t=>t.stop()); }
    screenStream = await navigator.mediaDevices.getDisplayMedia({video:true,audio:false});
    const video = document.getElementById('screen-video');
    const camV = document.getElementById('cam-video');
    camV.classList.remove('active');
    video.srcObject = screenStream;
    video.classList.add('active');
    document.getElementById('preview-area').classList.add('active');
    document.getElementById('preview-label').textContent = '📺 SCREEN SHARE';
    currentMode = 'screen';
    addSys('Screen share active. Tap "Analyze Screen" to ask JARVIS.');
    screenStream.getVideoTracks()[0].onended = ()=>stopPreview();
  } catch(e){
    addSys('Screen share cancelled or not supported, Sir.');
  }
}

// ── CAMERA ──
async function startCamera(){
  try{
    if(camStream){ camStream.getTracks().forEach(t=>t.stop()); }
    camStream = await navigator.mediaDevices.getUserMedia({video:{facingMode:'environment'},audio:false});
    const video = document.getElementById('cam-video');
    const scV = document.getElementById('screen-video');
    scV.classList.remove('active');
    video.srcObject = camStream;
    video.classList.add('active');
    document.getElementById('preview-area').classList.add('active');
    document.getElementById('preview-label').textContent = '📷 CAMERA';
    currentMode = 'cam';
    addSys('Camera active. Point at anything and tap "Analyze Screen".');
  } catch(e){
    addSys('Camera access denied, Sir. Please allow camera permission.');
  }
}

// ── STOP PREVIEW ──
function stopPreview(){
  if(screenStream){ screenStream.getTracks().forEach(t=>t.stop()); screenStream=null; }
  if(camStream){ camStream.getTracks().forEach(t=>t.stop()); camStream=null; }
  document.getElementById('preview-area').classList.remove('active');
  document.getElementById('screen-video').classList.remove('active');
  document.getElementById('cam-video').classList.remove('active');
  currentMode = null;
  addSys('Preview stopped.');
}

// ── CAPTURE & ANALYZE ──
async function captureAndAsk(){
  const videoEl = currentMode==='screen'
    ? document.getElementById('screen-video')
    : document.getElementById('cam-video');

  if(!currentMode || !videoEl.srcObject){
    addSys('Please start Screen Share or Camera first, Sir.');
    return;
  }

  // Capture frame
  const canvas = document.createElement('canvas');
  canvas.width = videoEl.videoWidth || 640;
  canvas.height = videoEl.videoHeight || 480;
  const ctx = canvas.getContext('2d');
  ctx.drawImage(videoEl, 0, 0);
  const base64 = canvas.toDataURL('image/jpeg', 0.7).split(',')[1];

  const prompt = currentMode==='screen'
    ? "Sir has shared their phone screen. Analyze what you see and tell Sir exactly what is happening on this screen and how to accomplish their goal. Be specific and helpful."
    : "Sir has shown you something with the camera. Describe what you see and help Sir understand it or solve any problem related to it.";

  addMsg('user', currentMode==='screen' ? '📺 [Screen shared — please analyze]' : '📷 [Camera image — please analyze]');
  askJarvis(prompt, base64);
}

// ── QUICK HELP ──
function quickHelp(){
  const inp = document.getElementById('txt-in');
  inp.value = 'আমি এটা কীভাবে করব? আমার screen দেখে বলো।';
  inp.focus();
  if(currentMode){
    captureAndAsk();
  } else {
    addSys('First tap "Screen Share" or "Camera", Sir.');
  }
}

// ── INIT ──
window.onload = async ()=>{
  if(synth.getVoices().length===0){
    await new Promise(r=>synth.addEventListener('voiceschanged',r,{once:true}));
  }
  addSys('— J.A.R.V.I.S ONLINE —');
  await askJarvis('Hello JARVIS. Greet me briefly and tell me the 3 main things you can help me with today.');
};
</script>
</body>
</html>
