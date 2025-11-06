<!doctype html>
<html lang="de">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>INNOVARE Offenbach — Mockup (Präsentation)</title>
  <meta name="description" content="Fiktives Leuchtturmprojekt — Science Center im Landkreis Offenbach (Mockup)" />
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
    body{margin:0;background:radial-gradient(ellipse at 10% 10%, rgba(167,139,250,0.06), transparent 10%), linear-gradient(180deg,#06101a 0%, #07101a 50%), var(--bg);color:#e6eef6;min-height:100vh}
    a{color:inherit}
    .container{max-width:1100px;margin:0 auto;padding:28px}

    .orb{position:fixed;border-radius:50%;filter:blur(60px);opacity:0.28;z-index:0}
    .orb.one{width:420px;height:420px;left:-80px;top:-80px;background:linear-gradient(135deg,var(--accent2),#ff7ab6)}
    .orb.two{width:360px;height:360px;right:-100px;bottom:-40px;background:linear-gradient(135deg,var(--accent1),#00b4ff)}

    header{position:relative;z-index:5;padding:18px 0}
    .nav{display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent1),var(--accent2));display:flex;align-items:center;justify-content:center;font-weight:800;color:#061021}
    nav ul{list-style:none;margin:0;padding:0;display:flex;gap:18px;align-items:center}
    nav a{color:var(--muted);text-decoration:none;font-weight:700}
    .notify{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:10px 14px;border-radius:12px;color:var(--muted)}

    .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:center;padding:48px 0;position:relative;z-index:6}
    .eyebrow{color:var(--accent1);font-weight:800;letter-spacing:0.08em}
    h1{font-size:clamp(1.8rem,4.4vw,3.2rem);margin:10px 0;line-height:1.02}
    .lead{color:var(--muted);max-width:60ch}
    .cta-row{display:flex;gap:12px;margin-top:18px}
    .btn{padding:12px 18px;border-radius:12px;font-weight:800;cursor:pointer;border:0}
    .btn.primary{background:linear-gradient(90deg,var(--accent1),var(--accent2));color:#061021}
    .btn.ghost{background:transparent;border:1px solid rgba(255,255,255,0.08);color:var(--muted)}

    .mock-card{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);border-radius:16px;padding:18px;box-shadow:0 12px 40px rgba(2,6,23,0.6);backdrop-filter: blur(6px)}

    .spheres{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:22px}
    .sphere{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);padding:18px;border-radius:14px;text-align:center;transition:transform .36s ease, box-shadow .36s ease}
    .sphere:hover{transform:translateY(-8px);box-shadow:0 18px 50px rgba(0,0,0,0.6)}
    .sphere h3{margin:10px 0}
    .sphere p{color:var(--muted);font-size:0.95rem}

    .news-grid{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:28px}
    .news-list .item{display:flex;gap:12px;align-items:flex-start;padding:12px;border-radius:12px;border:1px solid rgba(255,255,255,0.03);margin-bottom:10px}
    .news-list .meta{color:var(--muted);font-size:0.88rem}

    footer{margin-top:40px;padding:18px 0;color:var(--muted);font-size:0.9rem}

    @media (max-width:980px){.hero{grid-template-columns:1fr}.spheres{grid-template-columns:repeat(2,1fr)}.news-grid{grid-template-columns:1fr}}
    @media (max-width:600px){nav ul{display:none}.spheres{grid-template-columns:1fr}}
    .pulse{width:12px;height:12px;border-radius:50%;background:var(--accent1);box-shadow:0 0 18px rgba(110,231,246,0.6);animation:pulse 1.8s infinite}
    @keyframes pulse{0%{transform:scale(.9);opacity:0.9}50%{transform:scale(1.25);opacity:0.6}100%{transform:scale(.9);opacity:0.9}}
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
          <div style="font-size:0.85rem;color:var(--muted)">Leuchtturm‑Projekt — Präsentationsversion</div>
        </div>
      </div>

      <nav>
        <ul>
          <li><a href="#spheres">Themenwelten</a></li>
          <li><a href="#news">News</a></li>
          <li><a href="#kontakt">Kontakt</a></li>
        </ul>
      </nav>

      <div style="display:flex;gap:10px;align-items:center">
        <div class="notify"><span class="pulse" style="display:inline-block;margin-right:8px;vertical-align:middle"></span> COMING SOON</div>
      </div>
    </div>
  </header>

  <main class="container">
    <section class="hero">
      <div>
        <div class="eyebrow">Erleben. Forschen. Zukunft gestalten.</div>
        <h1>INNOVARE Offenbach — Das Science Center des Landkreises</h1>
        <p class="lead">Fiktives Leuchtturmprojekt: Interaktive Themenwelten zu Energie, Digitalisierung und Nachhaltigkeit. Entwickelt zur Förderung von Bildung, Wissenschaft und Innovation im Landkreis Offenbach.</p>

        <div class="cta-row">
          <button class="btn primary">Intro‑Video abspielen</button>
          <button class="btn ghost">Mehr erfahren</button>
        </div>

        <div class="mock-card" style="margin-top:20px;max-width:680px">
          <strong>Highlights</strong>
          <p style="margin:8px 0;color:var(--muted)">Interaktive Labore, immersive Projektionen und praxisnahe Workshops — visuell umgesetzt mit modernen Web‑Technologien.</p>
        </div>

        <div class="spheres" id="spheres">
          <div class="sphere">
            <h3>ENERGIA</h3>
            <p>Themenwelt: Energie & Umwelt — Experimente zu Solar‑, Wind‑ und Wasserstofftechnologien.</p>
          </div>
          <div class="sphere">
            <h3>DIGITA</h3>
            <p>Themenwelt: Digitalisierung & KI — spielerische Einführung in Programmierung und Robotik.</p>
          </div>
          <div class="sphere">
            <h3>NATURA</h3>
            <p>Themenwelt: Natur & Nachhaltigkeit — Biodiversität, Recycling und grüne Zukunftsideen.</p>
          </div>
        </div>
      </div>

      <aside>
        <div class="mock-card">
          <h3>Newsletter</h3>
          <p style="color:var(--muted)">Bleiben Sie informiert — tragen Sie Name & E‑Mail ein, um Updates zu erhalten.</p>
          <form style="display:grid;gap:8px;margin-top:12px">
            <input placeholder="Name" style="padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit">
            <input placeholder="E‑Mail" type="email" style="padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit">
            <button class="btn primary" type="button">Anmelden</button>
          </form>

          <div style="margin-top:14px;color:var(--muted);font-size:0.9rem">
            <strong>Kontakt</strong><br>
            Science Center INNOVARE Offenbach<br>
            Werner‑von‑Siemens‑Straße 12, 63075 Offenbach am Main
          </div>
        </div>

        <div class="mock-card" style="margin-top:16px">
          <h4>Partner & Sponsoren</h4>
          <div style="display:flex;flex-wrap:wrap;gap:8px;margin-top:10px">
            <div style="padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.03);font-weight:700">SAMSON AG</div>
            <div style="padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.03);font-weight:700">GKN Driveline</div>
            <div style="padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.03);font-weight:700">Hochschule RheinMain</div>
            <div style="padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.03);font-weight:700">Kreissparkasse Offenbach</div>
          </div>
        </div>
      </aside>
    </section>

    <section class="news-grid" id="news">
      <div>
        <h2>Aktuelles & Presse</h2>
        <div class="news-list">
          <div class="item">
            <div style="width:64px;height:64px;border-radius:8px;background:linear-gradient(90deg,var(--accent1),var(--accent2))"></div>
            <div>
              <div style="font-weight:800">Projektvorstellung im Kreishaus</div>
              <div class="meta">September 2025 — Pressemitteilung</div>
            </div>
          </div>

          <div class="item">
            <div style="width:64px;height:64px;border-radius:8px;background:linear-gradient(90deg,#ffb86b,#ff7ab6)"></div>
            <div>
              <div style="font-weight:800">Eröffnung des Info‑Labs</div>
              <div class="meta">August 2025 — Ankündigung</div>
            </div>
          </div>
        </div>
      </div>

      <aside class="mock-card">
        <h3>Besuch planen</h3>
        <p style="color:var(--muted)">Workshops und Führungen für Schulen, Vereine und Unternehmen im Landkreis Offenbach.</p>
        <div style="margin-top:12px;display:flex;gap:8px">
          <button class="btn primary">Tickets</button>
          <button class="btn ghost">Kontakt</button>
        </div>
      </aside>
    </section>

    <footer id="kontakt">
      <div style="display:flex;justify-content:space-between;align-items:center;gap:20px;flex-wrap:wrap">
        <div>© INNOVARE Offenbach — Mockup. Für Präsentationszwecke erstellt.</div>
        <div style="color:var(--muted)">Impressum • Datenschutz</div>
      </div>
    </footer>
  </main>

  <script>
    document.querySelectorAll('.btn').forEach(b=>b.addEventListener('click',()=>{alert('Dies ist eine Demo‑Interaktion — Präsentations‑Mockup.');}));
  </script>
</body>
</html>
