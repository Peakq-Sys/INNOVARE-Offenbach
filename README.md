<html lang="de">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />
<title>INNOVARE Offenbach — Science Center (Mockup)</title>
<meta name="description" content="Science Center im Landkreis Offenbach (Mockup)" />
<style>
:root{
  --bg:#070812;
  --card:#0f1724;
  --muted:#9aa4b2;
  --accent1:#00d4ff;
  --accent2:#a78bfa;
  --glass: rgba(255,255,255,0.06);
  --radius:16px;
  font-family: Inter, Roboto, system-ui, -apple-system, "Segoe UI", "Helvetica Neue", Arial;
}
*{box-sizing:border-box}
body{
  margin:0;
  background:radial-gradient(ellipse at 10% 10%, rgba(167,139,250,0.06), transparent 10%), linear-gradient(180deg,#06101a 0%, #07101a 50%), var(--bg);
  color:#e6eef6;
  min-height:100vh;
  scroll-behavior:smooth;
  font-size:1rem;
  line-height:1.5;
}
a{color:inherit;text-decoration:none}
.container{max-width:1100px;margin:0 auto;padding:28px}

.orb{position:fixed;border-radius:50%;filter:blur(60px);opacity:0.28;z-index:0}
.orb.one{width:420px;height:420px;left:-80px;top:-80px;background:linear-gradient(135deg,var(--accent2),#ff7ab6)}
.orb.two{width:360px;height:360px;right:-100px;bottom:-40px;background:linear-gradient(135deg,var(--accent1),#00b4ff)}

header{position:sticky;top:0;z-index:10;background:rgba(7,8,18,0.8);backdrop-filter:blur(12px);border-bottom:1px solid rgba(255,255,255,0.04)}
.nav{display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between}
.brand{display:flex;align-items:center;gap:12px}
.logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent1),var(--accent2));display:flex;align-items:center;justify-content:center;font-weight:800;color:#061021}
nav ul{list-style:none;margin:0;padding:0;display:flex;gap:18px;align-items:center;flex-wrap:wrap}
nav a{color:var(--muted);font-weight:700;transition:color .3s}
nav a:hover{color:var(--accent1)}
.notify{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px 14px;border-radius:12px;color:var(--muted)}

h1{font-size:clamp(1.8rem,5vw,3rem);margin:10px 0;line-height:1.1}
h2{font-size:clamp(1.25rem,4vw,2rem);margin-top:40px}
p, li{font-size:clamp(0.9rem,3.5vw,1rem)}
.lead{color:var(--muted);max-width:60ch}

.btn{padding:12px 18px;border-radius:12px;font-weight:800;cursor:pointer;border:0}
.btn.primary{background:linear-gradient(90deg,var(--accent1),var(--accent2));color:#061021}
.btn.ghost{background:transparent;border:1px solid rgba(255,255,255,0.08);color:var(--muted)}

.spheres{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px;margin-top:22px}
.sphere{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);padding:18px;border-radius:14px;text-align:center;transition:transform .36s ease, box-shadow .36s ease}
.sphere:hover{transform:translateY(-8px);box-shadow:0 18px 50px rgba(0,0,0,0.6)}
.sphere h3{margin:10px 0}
.sphere p{color:var(--muted);font-size:0.95rem}

.section{padding:80px 0;position:relative;z-index:5}
.section img{width:100%;height:auto;border-radius:16px;margin-top:20px}

footer{margin-top:80px;padding:18px 0;color:var(--muted);font-size:0.9rem;text-align:center}

.pulse{width:12px;height:12px;border-radius:50%;background:var(--accent1);box-shadow:0 0 18px rgba(110,231,246,0.6);animation:pulse 1.8s infinite}
@keyframes pulse{0%{transform:scale(.9);opacity:0.9}50%{transform:scale(1.25);opacity:0.6}100%{transform:scale(.9);opacity:0.9}}

@media (max-width:980px){
  .spheres{grid-template-columns:1fr;gap:12px}
}
@media (max-width:768px){
  nav ul{flex-direction:column;gap:12px;margin-top:8px}
  .container{padding:16px}
}
.credit {
  color: #9aa4b2; /* Grau */
  font-family: Calibri, Arial, sans-serif; 
  font-size: 0.625rem; 
  text-align: right; 
  margin-top: 6px; 
}
</style>
</head>
<body>
<div class="orb one" aria-hidden></div>
<div class="orb two" aria-hidden></div>
<header>
  <div class="container nav">
    <div class="brand">
      <div class="logo">IN</div>
      <div>
        <div style="font-weight:800">INNOVARE Offenbach</div>
        <div style="font-size:0.85rem;color:var(--muted)">Science Center — Mockup</div>
      </div>
    </div>
    <nav>
      <ul>
        <li><a href="#start">Start</a></li>
        <li><a href="#energia">Energia</a></li>
        <li><a href="#digita">Digita</a></li>
        <li><a href="#natura">Natura</a></li>
      </ul>
    </nav>
    <div style="display:flex;gap:10px;align-items:center">
      <div class="notify"><span class="pulse" style="display:inline-block;margin-right:8px;vertical-align:middle"></span>COMING SOON</div>
    </div>
  </div>
</header>
<main>
<section class="section" id="start">
  <div class="container">
    <h1>INNOVARE Offenbach — <br>Das Science Center der IKZ Offenbach</h1>
    <p class="lead">Interaktive Themenwelten zu Energie, Digitalisierung und Nachhaltigkeit.</p>
    <div class="spheres">
      <a href="#energia" class="sphere">
        <h3>ENERGIA</h3>
        <p>Energie & Umwelt — Solar-, Wind- und Wasserstoffexperimente.</p>
      </a>
      <a href="#digita" class="sphere">
        <h3>DIGITA</h3>
        <p>Digitalisierung & KI — Programmierung und Robotik spielerisch erleben.</p>
      </a>
      <a href="#natura" class="sphere">
        <h3>NATURA</h3>
        <p>Natur & Nachhaltigkeit — Biodiversität und grüne Zukunftsideen.</p>
      </a>
    </div>
  </div>
</section>

<section class="section" id="energia" style="background:rgba(255,255,255,0.02);">
  <div class="container">
    <h1>ENERGIA — Energie erleben und verstehen</h1>
    <p class="lead">Wie funktioniert eine Solarzelle? Warum dreht sich ein Windrad?</p>
    <img src="https://images.unsplash.com/photo-1613665813446-82a78c468a1d?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8N3x8c29sYXIlMjBwYW5lbHxlbnwwfHwwfHx8MA%3D%3D&auto=format&fit=crop&q=60&w=600auto=format&fit=crop&w=1100&q=80" alt="Solarpanel und Sonne">
    <p class="credit">© Nuno Marques on Unsplash</p>
    <h2>Highlights</h2>
    <ul>
      <li>Experimentierstationen für Solar- und Windenergie</li>
      <li>Interaktive Modelle zur Wasserstoffspeicherung</li>
      <li>Visualisierte Stromnetz-Simulation</li>
    </ul>
    <p><a href="#start" style="color:var(--accent1)">← Zurück</a></p>
  </div>
</section>

<section class="section" id="digita">
  <div class="container">
    <h1>DIGITA — Die Welt der Digitalisierung</h1>
    <p class="lead">Ob Robotik, künstliche Intelligenz oder 3D-Druck – spielerisch Technologie entdecken.</p>
    <img src="https://images.unsplash.com/photo-1518770660439-4636190af475?auto=format&fit=crop&w=1100&q=80" alt="Platine">
    <p class="credit">© Alexandre Debiève on Unsplash</p>
    <h2>Highlights</h2>
    <ul>
      <li>KI-Lab mit Bilderkennung und Sprachsteuerung</li>
      <li>Roboter-Workshops für Schulklassen</li>
      <li>Virtuelles Coding-Atelier für Einsteiger</li>
    </ul>
    <p><a href="#start" style="color:var(--accent1)">← Zurück</a></p>
  </div>
</section>

<section class="section" id="natura" style="background:rgba(255,255,255,0.02);">
  <div class="container">
    <h1>NATURA — Natur begreifen, Zukunft gestalten</h1>
    <p class="lead">Erlebnisstationen zu Recycling, Ökosystemen und nachhaltiger Stadtplanung.</p>
    <img src="https://images.unsplash.com/photo-1630586450644-684e310044dc?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=1170" alt="Natur und Nachhaltigkeit">
     <p class="credit">© Jaimy de Hon on Unsplash</p>
    <h2>Highlights</h2>
    <ul>
      <li>Recycling-Werkstatt zum Mitmachen</li>
      <li>Biodiversitätsgarten zum Erkunden</li>
      <li>Interaktive Karte „Grüne Städte der Zukunft“</li>
    </ul>
    <p><a href="#start" style="color:var(--accent1)">← Zurück</a></p>
  </div>
</section>

<footer>
  © INNOVARE Offenbach — Präsentations-Mockup • Impressum • Datenschutz
</footer>
</main>
</body>
</html>
