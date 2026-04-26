<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Wedding Invitation – Madhuri Priyanka & Yasoda Krishna</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400;1,500&family=Cinzel+Decorative:wght@400;700&family=Cinzel:wght@400;500;600&family=Great+Vibes&display=swap" rel="stylesheet">
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
:root {
  --g1:#1a3318; --g2:#2D4A2A; --g3:#4A7A42; --g4:#6B8F5E; --g5:#9FBF90;
  --g6:#B5C9A8; --g7:#D4E6C8; --g8:#EEF5E8;
  --gold1:#7A5C28; --gold2:#9A7B4F; --gold3:#C4A46B; --gold4:#E8CC90; --gold5:#F5E6C0;
  --cream:#FDFAF4; --cream2:#F7F2E8; --muted:#4A6844;
}
html { scroll-behavior: smooth; }
body {
  background: #0a1409;
  font-family: 'Cormorant Garamond', serif;
  min-height: 100vh;
  overflow-x: hidden;
}
body::before {
  content: '';
  position: fixed; inset: 0;
  background:
    radial-gradient(ellipse 80% 60% at 50% 0%, #1e3a1a 0%, transparent 70%),
    radial-gradient(ellipse 60% 40% at 20% 100%, #162814 0%, transparent 60%),
    #0a1409;
  z-index: 0;
}
#petals-canvas {
  position: fixed; top:0; left:0; width:100%; height:100%;
  pointer-events: none; z-index: 1;
}
.wrapper {
  position: relative; z-index: 2;
  display: flex; flex-direction: column; align-items: center;
  padding: 0 20px 80px;
}

/* ── OPENING ── */
.opening {
  width:100%; max-width:760px; min-height:100vh;
  display:flex; flex-direction:column; align-items:center; justify-content:center;
  text-align:center; padding:60px 20px; position:relative;
}
.mandala-wrap {
  width:260px; height:260px; position:relative; margin:0 auto 30px;
}
.mandala-outer { animation: spin 36s linear infinite; }
.mandala-inner { animation: spin 22s linear infinite reverse; transform-origin:50% 50%; }
@keyframes spin { to { transform: rotate(360deg); } }
.om-wrap {
  position:absolute; top:50%; left:50%; transform:translate(-50%,-50%);
  width:70px; height:70px; display:flex; align-items:center; justify-content:center;
}
.om-text {
  font-size:50px; color:var(--gold3);
  text-shadow: 0 0 20px rgba(196,164,107,0.7), 0 0 40px rgba(196,164,107,0.3);
  animation: glow-om 3s ease-in-out infinite;
  font-family: serif;
}
@keyframes glow-om {
  0%,100%{ text-shadow:0 0 20px rgba(196,164,107,0.6); }
  50%{ text-shadow:0 0 30px rgba(196,164,107,1),0 0 60px rgba(196,164,107,0.4); }
}
.open-blessing {
  font-family:'Cinzel',serif; font-size:10px; letter-spacing:4px;
  color:var(--g5); opacity:0; animation:fadeUp 1s 0.3s both;
}
.open-title {
  font-family:'Great Vibes',cursive; font-size:clamp(42px,8vw,68px); color:var(--gold4);
  text-shadow:0 0 40px rgba(232,204,144,0.5);
  opacity:0; animation:fadeUp 1.2s 0.6s both; margin:8px 0;
  line-height:1.1;
}
.open-hr {
  width:140px; height:1px; margin:16px auto;
  background:linear-gradient(90deg,transparent,var(--gold3),transparent);
  opacity:0; animation:fadeIn2 1s 1s both;
}
.open-names {
  font-family:'Great Vibes',cursive; font-size:clamp(30px,6vw,48px);
  color:var(--cream); opacity:0; animation:fadeUp 1.2s 1.2s both; line-height:1.3;
}
.open-date {
  font-family:'Cinzel',serif; font-size:11px; letter-spacing:3px;
  color:var(--g6); margin-top:14px; opacity:0; animation:fadeUp 1s 1.6s both;
}
.scroll-hint {
  margin-top:44px; opacity:0; animation:fadeIn2 1s 2.4s both;
  display:flex; flex-direction:column; align-items:center; gap:10px;
  color:var(--g5); font-family:'Cinzel',serif; font-size:9px; letter-spacing:3px;
}
.scroll-line {
  width:1px; height:48px;
  background:linear-gradient(to bottom,var(--gold3),transparent);
  animation:pulse-line 2s ease-in-out infinite;
}
@keyframes pulse-line { 0%,100%{opacity:.4;transform:scaleY(.8)} 50%{opacity:1;transform:scaleY(1)} }

/* ── PAGE ── */
.page {
  width:100%; max-width:740px; background:var(--cream);
  position:relative; overflow:hidden; border-radius:2px;
  box-shadow:0 0 0 1px rgba(181,201,168,0.25),0 24px 80px rgba(0,0,0,0.6);
}
/* animated gradient border */
.page-border {
  position:absolute; inset:-2px; z-index:0; border-radius:3px;
  background:linear-gradient(45deg,var(--g4),var(--gold3),var(--g5),var(--gold4),var(--g3),var(--gold3));
  background-size:300% 300%;
  animation:border-anim 8s ease infinite;
}
@keyframes border-anim {
  0%,100%{background-position:0% 50%} 50%{background-position:100% 50%}
}
.page-bg { position:absolute; inset:2px; background:var(--cream); border-radius:1px; z-index:0; }
.frame1 { position:absolute; inset:10px; border:0.5px solid rgba(181,201,168,0.45); pointer-events:none; z-index:5; }
.frame2 { position:absolute; inset:17px; border:0.5px solid rgba(196,164,107,0.2); pointer-events:none; z-index:5; }

/* Watermark botanical bg */
.watermark {
  position:absolute; inset:0; z-index:1; pointer-events:none; opacity:0.035;
  display:flex; align-items:center; justify-content:center;
}

.content { position:relative; z-index:2; padding:58px 68px 50px; text-align:center; }

/* Corners */
.corner { position:absolute; z-index:6; }
.corner.tl { top:0; left:0; }
.corner.tr { top:0; right:0; transform:scaleX(-1); }
.corner.bl { bottom:0; left:0; transform:scaleY(-1); }
.corner.br { bottom:0; right:0; transform:scale(-1,-1); }

/* ── Reveal ── */
.reveal { opacity:0; transform:translateY(28px); transition:opacity .9s ease,transform .9s ease; }
.reveal.on { opacity:1; transform:translateY(0); }
.rl { opacity:0; transform:translateX(-28px); transition:opacity .9s ease,transform .9s ease; }
.rl.on { opacity:1; transform:translateX(0); }
.rr { opacity:0; transform:translateX(28px); transition:opacity .9s ease,transform .9s ease; }
.rr.on { opacity:1; transform:translateX(0); }
.d1{transition-delay:.05s} .d2{transition-delay:.15s} .d3{transition-delay:.25s}
.d4{transition-delay:.35s} .d5{transition-delay:.45s}

/* ── Typography ── */
.blessing-tag {
  font-family:'Cinzel',serif; font-size:10.5px; letter-spacing:4px;
  color:var(--gold2); display:inline-block; position:relative;
}
.blessing-tag::before,.blessing-tag::after{ content:'✦'; color:var(--gold3); margin:0 8px; }

.gold-rule {
  display:flex; align-items:center; gap:14px; margin:14px auto; width:85%;
}
.gold-rule::before,.gold-rule::after {
  content:''; flex:1; height:0.5px;
  background:linear-gradient(90deg,transparent,var(--gold3),transparent);
}
.gold-rule span { color:var(--gold3); font-size:15px; }

.gp-line { font-size:13px; color:var(--muted); font-style:italic; }

.host-name {
  font-family:'Cinzel',serif; font-size:14px; color:var(--g2);
  letter-spacing:1.5px; line-height:2.1;
}
.host-sub { font-size:13px; color:var(--muted); font-style:italic; line-height:1.9; margin-top:5px; }

/* ── Medallion ── */
.med-wrap {
  margin:26px auto; position:relative; width:290px; height:290px;
}
.med-r1,.med-r2,.med-r3 {
  position:absolute; inset:0; border-radius:50%;
  border:1px solid transparent;
}
.med-r1 {
  background:linear-gradient(var(--cream),var(--cream)) padding-box,
             conic-gradient(var(--gold3),var(--g5),var(--gold4),var(--g6),var(--gold3)) border-box;
  animation:spin 14s linear infinite;
}
.med-r2 {
  inset:9px;
  background:linear-gradient(var(--cream),var(--cream)) padding-box,
             conic-gradient(var(--g5),var(--gold3),var(--g6),var(--gold4),var(--g5)) border-box;
  animation:spin 20s linear infinite reverse;
}
.med-r3 { inset:17px; border:0.5px solid rgba(181,201,168,0.5); }
.med-glow {
  position:absolute; inset:22px; border-radius:50%;
  background:radial-gradient(circle,rgba(181,201,168,0.28) 0%,transparent 70%);
  animation:glow-med 3.5s ease-in-out infinite;
}
@keyframes glow-med {
  0%,100%{opacity:.6;transform:scale(.95)} 50%{opacity:1;transform:scale(1.06)}
}
.med-core {
  position:absolute; inset:22px; border-radius:50%;
  background:linear-gradient(150deg,#F6FBF2,#EAF3E2,#F2F9EE);
  display:flex; flex-direction:column; align-items:center; justify-content:center;
  padding:18px;
}
.bride { font-family:'Great Vibes',cursive; font-size:32px; color:var(--g2); line-height:1.1; }
.qual { font-size:9px; color:var(--g4); font-style:italic; letter-spacing:.5px; margin-top:1px; }
.amp {
  font-family:'Great Vibes',cursive; font-size:48px; color:var(--g4); line-height:1; margin:1px 0;
  animation:amp-glow 3s ease-in-out infinite;
}
@keyframes amp-glow {
  0%,100%{color:var(--g4)} 50%{color:var(--g3);text-shadow:0 0 12px rgba(107,143,94,.45)}
}
.groom { font-family:'Great Vibes',cursive; font-size:32px; color:var(--g2); line-height:1.1; }

/* orbiting leaves */
.orbit-ring {
  position:absolute; inset:-12px; border-radius:50%;
  animation:spin 22s linear infinite; pointer-events:none;
}
.orbit-leaf {
  position:absolute; width:9px; height:14px;
  background:radial-gradient(ellipse,rgba(181,201,168,.85),rgba(107,143,94,.25));
  border-radius:50% 50% 50% 0; transform-origin:50% 100%;
}

/* ── Parent note ── */
.parent-note {
  font-size:13px; color:var(--muted); font-style:italic; line-height:1.85;
  background:rgba(238,245,232,.5); border:.5px solid var(--g7); border-radius:5px;
  padding:11px 18px; margin:10px 0 18px;
}

/* ── Section heading ── */
.sec-head {
  font-family:'Cinzel Decorative',serif; font-size:10.5px; letter-spacing:4px;
  color:var(--gold2); margin:4px 0 14px;
}

/* ── Countdown ── */
.cd-wrap {
  background:linear-gradient(135deg,#1e3a18,#152a12);
  border-radius:8px; padding:22px; margin:4px 0 16px;
  position:relative; overflow:hidden;
}
.cd-wrap::before {
  content:''; position:absolute; inset:1px; border-radius:7px;
  border:.5px solid rgba(181,201,168,.25); pointer-events:none;
}
.cd-wrap::after {
  content:''; position:absolute; inset:0;
  background:radial-gradient(ellipse 80% 60% at 50% 0%,rgba(107,143,94,.12),transparent);
  pointer-events:none;
}
.cd-label {
  font-family:'Cinzel',serif; font-size:9px; letter-spacing:3.5px;
  color:var(--g6); margin-bottom:14px; position:relative; z-index:1;
}
.cd-units { display:flex; justify-content:center; gap:14px; position:relative; z-index:1; }
.cd-unit { text-align:center; min-width:52px; }
.cd-num {
  font-family:'Cinzel Decorative',serif; font-size:30px; color:var(--gold4); line-height:1;
  text-shadow:0 0 20px rgba(232,204,144,.45);
}
.cd-lbl { font-family:'Cinzel',serif; font-size:8px; letter-spacing:2px; color:var(--g5); margin-top:5px; }
.cd-sep { font-size:26px; color:var(--gold3); line-height:1.2; opacity:.7; animation:blink 1s step-end infinite; }
@keyframes blink { 0%,100%{opacity:.7} 50%{opacity:.15} }

/* ── Events ── */
.events-grid { display:grid; grid-template-columns:1fr 1fr 1fr; gap:12px; margin:0 0 14px; }
.ev-card {
  background:linear-gradient(155deg,var(--g8),#E5F0DC);
  border:.5px solid var(--g6); border-radius:7px; padding:18px 10px;
  text-align:center; position:relative; overflow:hidden;
  transition:transform .3s ease,box-shadow .3s ease; cursor:default;
}
.ev-card::after {
  content:''; position:absolute; top:0;left:0;right:0; height:2px;
  background:linear-gradient(90deg,var(--g5),var(--gold3),var(--g5));
  opacity:0; transition:opacity .3s;
}
.ev-card:hover { transform:translateY(-5px); box-shadow:0 10px 28px rgba(45,74,42,.15); }
.ev-card:hover::after { opacity:1; }
.ev-icon {
  width:50px; height:50px; border-radius:50%;
  background:linear-gradient(135deg,rgba(181,201,168,.45),rgba(107,143,94,.2));
  border:.5px solid var(--g6); display:flex; align-items:center; justify-content:center;
  font-size:23px; margin:0 auto 9px;
  transition:transform .3s ease;
}
.ev-card:hover .ev-icon { transform:scale(1.12) rotate(6deg); }
.ev-name { font-family:'Cinzel',serif; font-size:10px; color:var(--g2); letter-spacing:1.5px; margin-bottom:6px; }
.ev-detail { font-size:11.5px; color:var(--muted); line-height:1.65; font-style:italic; }
.ev-date {
  font-family:'Cinzel',serif; font-size:9px; color:var(--gold2); margin-top:7px;
  background:rgba(196,164,107,.12); border:.5px solid rgba(196,164,107,.3);
  border-radius:3px; padding:3px 7px; display:inline-block; letter-spacing:.3px;
}

/* ── Venue ── */
.venue {
  background:linear-gradient(135deg,var(--g8),#E8F2DF);
  border:.5px solid var(--g6); border-left:3px solid var(--g4);
  border-radius:7px; padding:18px 22px; margin:14px 0;
  display:flex; align-items:center; gap:16px; text-align:left;
  position:relative; overflow:hidden;
  transition:transform .3s ease;
}
.venue:hover { transform:translateX(5px); }
.venue::after { content:'🌿'; position:absolute; right:16px; bottom:10px; font-size:34px; opacity:.12; }
.venue-icon {
  width:54px; height:54px; border-radius:50%;
  background:linear-gradient(135deg,var(--g4),var(--g3));
  display:flex; align-items:center; justify-content:center;
  font-size:25px; flex-shrink:0; box-shadow:0 4px 14px rgba(45,74,42,.25);
}
.venue-lbl { font-family:'Cinzel',serif; font-size:9px; letter-spacing:3px; color:var(--g4); margin-bottom:4px; }
.venue-nm { font-family:'Cormorant Garamond',serif; font-size:21px; color:var(--g2); font-weight:500; }
.venue-addr { font-size:13px; color:var(--muted); font-style:italic; margin-top:2px; }
.venue-time {
  font-family:'Cinzel',serif; font-size:10px; color:var(--gold2);
  margin-top:6px; letter-spacing:.8px;
}
.venue-time::before { content:'📅 '; }

/* ── Dinner ── */
.dinner {
  background:linear-gradient(135deg,rgba(245,230,192,.28),rgba(232,204,144,.14));
  border:.5px solid rgba(196,164,107,.35); border-radius:6px;
  padding:12px 18px; font-size:13px; font-style:italic;
  color:var(--gold1); display:flex; align-items:center; gap:10px; margin:6px 0;
}

/* ── Footer ── */
.footer {
  margin-top:20px; padding:22px;
  background:linear-gradient(135deg,var(--g8),#EBF3E6);
  border:.5px solid var(--g6); border-radius:7px; text-align:center;
  font-size:12px; color:var(--muted); font-style:italic; line-height:1.9;
}
.footer-script { font-family:'Great Vibes',cursive; font-size:30px; color:var(--g2); font-style:normal; }
.footer-name { font-family:'Cinzel',serif; font-size:12px; color:var(--g2); font-style:normal; letter-spacing:.5px; line-height:1.8; margin-bottom:10px; }

/* ── Bottom vine ── */
.bot-vine { margin-top:26px; text-align:center; }
.bot-vine svg { width:320px; height:42px; opacity:.55; }

/* ── Keyframes ── */
@keyframes fadeUp { from{opacity:0;transform:translateY(20px)} to{opacity:1;transform:translateY(0)} }
@keyframes fadeIn2 { from{opacity:0} to{opacity:1} }

@media(max-width:580px){
  .content{padding:42px 28px 38px}
  .events-grid{grid-template-columns:1fr}
  .med-wrap{width:230px;height:230px}
  .med-core{inset:18px}
  .bride,.groom{font-size:26px} .amp{font-size:40px}
  .cd-num{font-size:24px}
}
@media print{
  body{background:#fff} #petals-canvas{display:none} .opening{display:none}
  .page-border{display:none} .page{box-shadow:none}
}
</style>
</head>
<body>

<canvas id="petals-canvas"></canvas>

<div class="wrapper">

<!-- ═══ OPENING ═══ -->
<div class="opening">
  <div class="mandala-wrap">
    <svg width="260" height="260" viewBox="0 0 260 260">
      <!-- outer rings -->
      <circle cx="130" cy="130" r="126" fill="none" stroke="rgba(181,201,168,.22)" stroke-width=".5"/>
      <circle cx="130" cy="130" r="118" fill="none" stroke="rgba(196,164,107,.15)" stroke-width=".5"/>
      <!-- outer petals -->
      <g class="mandala-outer" style="transform-origin:130px 130px">
        <g transform="translate(130,130)">
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(0) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(30) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(60) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(90) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(120) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(150) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(180) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(210) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(240) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(270) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(300) translate(0,-90)"/>
          <ellipse rx="9" ry="28" fill="rgba(107,143,94,.28)" transform="rotate(330) translate(0,-90)"/>
        </g>
      </g>
      <!-- inner petals counter-rotate -->
      <g class="mandala-inner" style="transform-origin:130px 130px">
        <g transform="translate(130,130)">
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(15) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(45) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(75) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(105) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(135) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(165) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(195) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(225) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(255) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(285) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(315) translate(0,-58)"/>
          <ellipse rx="6" ry="20" fill="rgba(196,164,107,.32)" transform="rotate(345) translate(0,-58)"/>
        </g>
      </g>
      <circle cx="130" cy="130" r="36" fill="rgba(12,22,10,.85)" stroke="rgba(196,164,107,.45)" stroke-width=".7"/>
    </svg>
    <div class="om-wrap"><span class="om-text">ॐ</span></div>
  </div>
  <p class="open-blessing">WITH DIVINE BLESSINGS</p>
  <h1 class="open-title">Dadi's Wedding Invitation</h1>
  <div class="open-hr"></div>
  <div class="open-names">Madhuri Priyanka<br>&amp; Yasoda Krishna</div>
  <p class="open-date">THURSDAY · 7TH MAY 2026 · MUNAGAPAKA</p>
  <div class="scroll-hint">
    <span>SCROLL TO VIEW</span>
    <div class="scroll-line"></div>
  </div>
</div>

<!-- ═══ INVITATION PAGE ═══ -->
<div class="page">
  <div class="page-border"></div>
  <div class="page-bg"></div>
  <div class="frame1"></div>
  <div class="frame2"></div>

  <!-- Watermark -->
  <div class="watermark">
    <svg width="400" height="400" viewBox="0 0 400 400" fill="none">
      <g transform="translate(200,200)">
        <ellipse rx="12" ry="60" fill="#2D4A2A" transform="rotate(0) translate(0,-120)"/>
        <ellipse rx="12" ry="60" fill="#2D4A2A" transform="rotate(45) translate(0,-120)"/>
        <ellipse rx="12" ry="60" fill="#2D4A2A" transform="rotate(90) translate(0,-120)"/>
        <ellipse rx="12" ry="60" fill="#2D4A2A" transform="rotate(135) translate(0,-120)"/>
        <ellipse rx="12" ry="60" fill="#2D4A2A" transform="rotate(180) translate(0,-120)"/>
        <ellipse rx="12" ry="60" fill="#2D4A2A" transform="rotate(225) translate(0,-120)"/>
        <ellipse rx="12" ry="60" fill="#2D4A2A" transform="rotate(270) translate(0,-120)"/>
        <ellipse rx="12" ry="60" fill="#2D4A2A" transform="rotate(315) translate(0,-120)"/>
      </g>
      <circle cx="200" cy="200" r="60" fill="none" stroke="#2D4A2A" stroke-width="1"/>
    </svg>
  </div>

  <!-- Corners -->
  <svg class="corner tl" width="115" height="115" viewBox="0 0 115 115" fill="none">
    <path d="M8 107 Q8 8 107 8" stroke="#6B8F5E" stroke-width=".7" fill="none" opacity=".35"/>
    <path d="M3 107 Q3 3 107 3" stroke="#C4A46B" stroke-width=".4" fill="none" opacity=".25"/>
    <ellipse cx="30" cy="30" rx="17" ry="9" fill="#6B8F5E" opacity=".22" transform="rotate(-35 30 30)"/>
    <ellipse cx="19" cy="52" rx="13" ry="6" fill="#9FBF90" opacity=".18" transform="rotate(-20 19 52)"/>
    <ellipse cx="52" cy="19" rx="13" ry="6" fill="#9FBF90" opacity=".18" transform="rotate(-60 52 19)"/>
    <circle cx="32" cy="32" r="4.5" fill="#B5C9A8" opacity=".5"/>
    <circle cx="19" cy="54" r="2.5" fill="#6B8F5E" opacity=".4"/>
    <circle cx="54" cy="19" r="2.5" fill="#6B8F5E" opacity=".4"/>
    <path d="M23 23 Q34 14 42 25 Q34 36 23 23Z" fill="#6B8F5E" opacity=".28"/>
    <path d="M10 38 Q20 27 30 37 Q21 47 10 38Z" fill="#9FBF90" opacity=".22"/>
    <path d="M38 10 Q47 21 36 30 Q27 21 38 10Z" fill="#9FBF90" opacity=".22"/>
    <circle cx="58" cy="12" r="1.5" fill="#C4A46B" opacity=".38"/>
    <circle cx="12" cy="58" r="1.5" fill="#C4A46B" opacity=".38"/>
  </svg>
  <svg class="corner tr" width="115" height="115" viewBox="0 0 115 115" fill="none">
    <path d="M8 107 Q8 8 107 8" stroke="#6B8F5E" stroke-width=".7" fill="none" opacity=".35"/>
    <path d="M3 107 Q3 3 107 3" stroke="#C4A46B" stroke-width=".4" fill="none" opacity=".25"/>
    <ellipse cx="30" cy="30" rx="17" ry="9" fill="#6B8F5E" opacity=".22" transform="rotate(-35 30 30)"/>
    <ellipse cx="19" cy="52" rx="13" ry="6" fill="#9FBF90" opacity=".18" transform="rotate(-20 19 52)"/>
    <ellipse cx="52" cy="19" rx="13" ry="6" fill="#9FBF90" opacity=".18" transform="rotate(-60 52 19)"/>
    <circle cx="32" cy="32" r="4.5" fill="#B5C9A8" opacity=".5"/>
    <path d="M23 23 Q34 14 42 25 Q34 36 23 23Z" fill="#6B8F5E" opacity=".28"/>
  </svg>
  <svg class="corner bl" width="115" height="115" viewBox="0 0 115 115" fill="none">
    <path d="M8 107 Q8 8 107 8" stroke="#6B8F5E" stroke-width=".7" fill="none" opacity=".35"/>
    <path d="M3 107 Q3 3 107 3" stroke="#C4A46B" stroke-width=".4" fill="none" opacity=".25"/>
    <ellipse cx="30" cy="30" rx="17" ry="9" fill="#6B8F5E" opacity=".22" transform="rotate(-35 30 30)"/>
    <circle cx="32" cy="32" r="4.5" fill="#B5C9A8" opacity=".5"/>
    <path d="M23 23 Q34 14 42 25 Q34 36 23 23Z" fill="#6B8F5E" opacity=".28"/>
  </svg>
  <svg class="corner br" width="115" height="115" viewBox="0 0 115 115" fill="none">
    <path d="M8 107 Q8 8 107 8" stroke="#6B8F5E" stroke-width=".7" fill="none" opacity=".35"/>
    <path d="M3 107 Q3 3 107 3" stroke="#C4A46B" stroke-width=".4" fill="none" opacity=".25"/>
    <ellipse cx="30" cy="30" rx="17" ry="9" fill="#6B8F5E" opacity=".22" transform="rotate(-35 30 30)"/>
    <circle cx="32" cy="32" r="4.5" fill="#B5C9A8" opacity=".5"/>
    <path d="M23 23 Q34 14 42 25 Q34 36 23 23Z" fill="#6B8F5E" opacity=".28"/>
  </svg>

  <div class="content">

    <p class="blessing-tag reveal d1">With Divine Blessings</p>
    <div class="gold-rule reveal d2"><span>✦</span></div>
    <p class="gp-line reveal d2">Sri Dadi Kammayya · Smt. Paradesammma garu</p>

    <div class="reveal d3" style="margin:12px 0 18px">
      <p class="host-name">Sri Dadi Kesava Varaha Narasimha Murthy</p>
      <p class="host-name">&amp; Smt. Nagamani</p>
      <p class="host-sub">solicit your gracious presence with family and friends<br>on the auspicious occasion of the marriage of their only son</p>
    </div>

    <!-- Medallion -->
    <div class="med-wrap reveal d4">
      <div class="med-r1"></div>
      <div class="med-r2"></div>
      <div class="med-r3"></div>
      <div class="med-glow"></div>
      <div class="orbit-ring" id="orbitRing"></div>
      <div class="med-core">
        <div class="bride">Madhuri Priyanka</div>
        <div class="qual">M.B.A. (fm)</div>
        <div class="amp">&amp;</div>
        <div class="groom">Yasoda Krishna</div>
        <div class="qual">M.B.A. (fin)</div>
      </div>
    </div>

    <p class="parent-note reveal d3">
      Daughter of Sri Tekkam Sri Ram – Smt. Bhagya Lakshmi garu<br>
      of Mamangapaka village
    </p>

    <div class="gold-rule reveal"><span>❧</span></div>

    <!-- Countdown -->
    <div class="cd-wrap reveal">
      <p class="cd-label">COUNTING DOWN TO THE CELEBRATION</p>
      <div class="cd-units">
        <div class="cd-unit"><div class="cd-num" id="cdD">00</div><div class="cd-lbl">DAYS</div></div>
        <div class="cd-sep">:</div>
        <div class="cd-unit"><div class="cd-num" id="cdH">00</div><div class="cd-lbl">HRS</div></div>
        <div class="cd-sep">:</div>
        <div class="cd-unit"><div class="cd-num" id="cdM">00</div><div class="cd-lbl">MINS</div></div>
        <div class="cd-sep">:</div>
        <div class="cd-unit"><div class="cd-num" id="cdS">00</div><div class="cd-lbl">SECS</div></div>
      </div>
    </div>

    <div class="gold-rule reveal"><span>✿</span></div>
    <p class="sec-head reveal">Events &amp; Ceremonies</p>

    <!-- Events -->
    <div class="events-grid">
      <div class="ev-card rl d2">
        <div class="ev-icon">🪔</div>
        <div class="ev-name">Pellikuthuru</div>
        <div class="ev-detail">At our residence, near Tulasi Kalyana Mandapam, Munagapaka</div>
        <div class="ev-date">Thu 7 May 2026 · 10:43 AM</div>
      </div>
      <div class="ev-card reveal d3">
        <div class="ev-icon">💍</div>
        <div class="ev-name">Muhurtham</div>
        <div class="ev-detail">Tulasi Kalyana Mandapam · Dharur Lagnam · 10:30–43 hrs</div>
        <div class="ev-date">Thu 7 May 2026 · Night 10:30</div>
      </div>
      <div class="ev-card rr d2">
        <div class="ev-icon">🌸</div>
        <div class="ev-name">Pendlikathera</div>
        <div class="ev-detail">Mamangapaka Village · Smt. Bhagya Lakshmi garu</div>
        <div class="ev-date">Thu 7 May 2026 · 8:00 AM</div>
      </div>
    </div>

    <!-- Venue -->
    <div class="venue reveal">
      <div class="venue-icon">🏛️</div>
      <div>
        <div class="venue-lbl">VENUE</div>
        <div class="venue-nm">Tulasi Kalyana Mandapam</div>
        <div class="venue-addr">Pulapu Veedhi, Munagapaka</div>
        <div class="venue-time">Thursday, 7th May 2026</div>
      </div>
    </div>

    <!-- Dinner -->
    <div class="dinner reveal">
      <span>🍽️</span>
      <span>Dinner: Thursday 7th May 2026 · 7 PM onwards at the marriage venue</span>
    </div>

    <div class="gold-rule reveal"><span>❧</span></div>

    <!-- Footer -->
    <div class="footer reveal">
      <div class="footer-script">With Warmest Regards,</div>
      <div class="footer-name">
        Sri Dadi Kesava Varaha Narasimha Murthy &amp; Smt. Nagamani
      </div>
      <em>With Best Compliments from: Sri P. Narasinga Rao · Sri P. Nooka Praveen · Sri P. Lawyers ·
      Sri D. Vijaya Naidu · Smt. Lakshmi · Sri D. Srinivas Rao · Smt. Usha Kumari ·
      Sri D. Uday Kumar · Smt. Lakshmi · Sri K. Raju · K. Ramayamma ·
      Sri D. Muralikrishna Naidu · Smt. Raja · K. Kirupa and near and dear ones</em>
    </div>

    <!-- Bottom vine -->
    <div class="bot-vine reveal">
      <svg viewBox="0 0 320 42" fill="none">
        <line x1="0" y1="21" x2="320" y2="21" stroke="rgba(181,201,168,.4)" stroke-width=".5"/>
        <ellipse cx="44" cy="21" rx="18" ry="9" fill="rgba(107,143,94,.22)" transform="rotate(-20 44 21)"/>
        <ellipse cx="76" cy="14" rx="14" ry="7" fill="rgba(107,143,94,.26)" transform="rotate(-10 76 14)"/>
        <circle cx="96" cy="21" r="5" fill="rgba(181,201,168,.42)"/>
        <circle cx="96" cy="21" r="2" fill="rgba(107,143,94,.6)"/>
        <text x="160" y="27" text-anchor="middle" font-size="16" fill="rgba(196,164,107,.65)" font-family="serif">✦</text>
        <circle cx="160" cy="21" r="8" fill="none" stroke="rgba(196,164,107,.35)" stroke-width=".5"/>
        <ellipse cx="224" cy="21" rx="14" ry="7" fill="rgba(107,143,94,.26)" transform="rotate(10 224 21)"/>
        <ellipse cx="256" cy="14" rx="18" ry="9" fill="rgba(107,143,94,.22)" transform="rotate(20 256 14)"/>
        <circle cx="276" cy="21" r="5" fill="rgba(181,201,168,.42)"/>
        <circle cx="276" cy="21" r="2" fill="rgba(107,143,94,.6)"/>
      </svg>
    </div>

  </div><!-- /content -->
</div><!-- /page -->
</div><!-- /wrapper -->

<script>
/* ── Falling petals canvas ── */
(function(){
  const c=document.getElementById('petals-canvas'),x=c.getContext('2d');
  let W,H,petals=[],frame=0;
  function resize(){W=c.width=innerWidth;H=c.height=innerHeight;}
  resize(); addEventListener('resize',resize);
  const COLS=['rgba(181,201,168,.7)','rgba(107,143,94,.5)','rgba(159,191,144,.6)',
               'rgba(196,164,107,.42)','rgba(232,204,144,.38)','rgba(212,224,204,.58)'];
  function spawn(){
    const sz=7+Math.random()*11;
    petals.push({
      x:Math.random()*W, y:-20,
      vx:(Math.random()-.5)*1.4, vy:.6+Math.random()*1.1,
      rot:Math.random()*Math.PI*2, vr:(Math.random()-.5)*.038,
      sz, col:COLS[Math.floor(Math.random()*COLS.length)],
      sa:.6+Math.random()*1.4, sf:.012+Math.random()*.018,
      so:Math.random()*Math.PI*2, t:0,
      type:Math.random()>.5?0:1
    });
  }
  function draw(p){
    x.save(); x.translate(p.x,p.y); x.rotate(p.rot);
    x.fillStyle=p.col; x.beginPath();
    if(p.type===0){
      x.ellipse(0,0,p.sz*.38,p.sz,0,0,Math.PI*2);
    }else{
      x.moveTo(0,-p.sz);
      x.bezierCurveTo(p.sz*.58,-p.sz*.5,p.sz*.4,p.sz*.3,0,p.sz);
      x.bezierCurveTo(-p.sz*.4,p.sz*.3,-p.sz*.58,-p.sz*.5,0,-p.sz);
    }
    x.fill(); x.restore();
  }
  function loop(){
    x.clearRect(0,0,W,H); frame++;
    if(frame%20===0&&petals.length<40) spawn();
    petals=petals.filter(p=>p.y<H+30);
    petals.forEach(p=>{
      p.t++; p.x+=p.vx+Math.sin(p.t*p.sf+p.so)*p.sa;
      p.y+=p.vy; p.rot+=p.vr; draw(p);
    });
    requestAnimationFrame(loop);
  }
  loop();
})();

/* ── Countdown ── */
(function(){
  const target=new Date('2026-05-07T10:43:00+05:30');
  function pad(n){return String(n).padStart(2,'0');}
  function tick(){
    const diff=target-Date.now();
    if(diff<=0){
      ['cdD','cdH','cdM','cdS'].forEach(id=>document.getElementById(id).textContent='00');
      return;
    }
    document.getElementById('cdD').textContent=pad(Math.floor(diff/86400000));
    document.getElementById('cdH').textContent=pad(Math.floor((diff%86400000)/3600000));
    document.getElementById('cdM').textContent=pad(Math.floor((diff%3600000)/60000));
    document.getElementById('cdS').textContent=pad(Math.floor((diff%60000)/1000));
  }
  tick(); setInterval(tick,1000);
})();

/* ── Scroll reveal ── */
(function(){
  const els=document.querySelectorAll('.reveal,.rl,.rr');
  const ob=new IntersectionObserver(entries=>{
    entries.forEach(e=>{if(e.isIntersecting)e.target.classList.add('on');});
  },{threshold:.12});
  els.forEach(el=>ob.observe(el));
})();

/* ── Orbiting leaves on medallion ── */
(function(){
  const ring=document.getElementById('orbitRing');
  const n=10;
  for(let i=0;i<n;i++){
    const div=document.createElement('div');
    div.className='orbit-leaf';
    const a=(i/n)*360, r=138;
    const rad=a*Math.PI/180;
    const x=157+r*Math.cos(rad)-4.5;
    const y=157+r*Math.sin(rad)-7;
    div.style.cssText=`left:${x}px;top:${y}px;transform:rotate(${a+90}deg);`;
    ring.appendChild(div);
  }
})();
</script>
</body>
</html>
