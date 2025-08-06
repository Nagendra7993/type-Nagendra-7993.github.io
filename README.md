# type-Nagendra-7993.github.io
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Mallireddypalli — Village Development</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="hero">
    <div class="container hero-grid">
      <div class="hero-text">
        <h1>Mallireddypalli</h1>
        <p class="lead">Preserving tradition. Building a brighter future.</p>
        <p class="bio">I’m <strong>A Nagendra</strong>. I love my village — its culture, temples, and the people. Join us in community-led development and cultural revival.</p>
        <p class="cta-row">
          <a href="#projects" class="btn">Our Projects</a>
          <a href="#contact" class="btn ghost">Contact</a>
        </p>
      </div>
    </div>
  </header>

  <main class="container">
    <section id="about" class="card">
      <h2>About the Village</h2>
      <p>Mallireddypalli is rooted in strong traditions — our festivals, temples, music and crafts shape daily life. We focus on projects that support education, infrastructure, and cultural preservation.</p>
      <ul class="points">
        <li>Protect and restore local temples</li>
        <li>Encourage traditional arts &amp; crafts</li>
        <li>Improve basic infrastructure & sanitation</li>
        <li>Support youth education and skills</li>
      </ul>
    </section>

    <section id="projects" class="card">
      <h2>Development Projects</h2>
      <div class="grid">
        <article>
          <h3>Temple Conservation</h3>
          <p>Planning restorations, community cleanups and rituals maintenance.</p>
        </article>
        <article>
          <h3>Education & Skills</h3>
          <p>After-school programs, adult literacy drives and vocational training.</p>
        </article>
        <article>
          <h3>Sanitation & Water</h3>
          <p>Village pond cleanup, safe water access and sanitation awareness.</p>
        </article>
      </div>
    </section>

    <section id="culture" class="card">
      <h2>Culture & Traditions</h2>
      <p>Festivals, music, bhajans, and local ceremonies are our heart. We document traditions and encourage younger generations to learn them.</p>
      <div class="gallery">
        <div class="gcell">Temple</div>
        <div class="gcell">Festival</div>
        <div class="gcell">Music</div>
      </div>
    </section>

    <section id="contact" class="card">
      <h2>Contact</h2>
      <p><strong>A Nagendra</strong></p>
      <p>Phone: <a href="tel:+917993717142">+91 79937 17142</a></p>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container">
      <p>© <span id="year"></span> Mallireddypalli — Village Development • Built by A Nagendra</p>
    </div>
  </footer>

  <script src="script.js"></script>
</body>
</html>
:root{
  --bg: #fff;
  --text: #222;
  --muted:#666;
  --accent:#d97706; /* saffron/orange */
  --accent2:#166534; /* deep green */
  --card:#fff7ed;
  --max-width:1000px;
  font-family: "Segoe UI", Roboto, Arial, sans-serif;
}
*{box-sizing:border-box}
body{margin:0;background:linear-gradient(180deg,#fff 0%,#fffdf7 100%);color:var(--text);line-height:1.55}
.container{max-width:var(--max-width);margin:0 auto;padding:24px}
.hero{background:linear-gradient(90deg, rgba(217,119,6,0.06), rgba(22,101,52,0.03));padding:36px 0;border-bottom:1px solid rgba(0,0,0,0.04)}
.hero-grid{display:grid;grid-template-columns:1fr;gap:24px;align-items:center;text-align:center}
h1{margin:0;font-size:clamp(28px,4vw,40px);color:var(--accent2)}
.lead{color:var(--muted);margin:8px 0 12px}
.bio{margin:0 0 12px}
.btn{display:inline-block;padding:10px 14px;border-radius:8px;text-decoration:none;background:var(--accent);color:#fff;margin-right:8px}
.btn.ghost{background:transparent;border:1px solid rgba(22,101,52,0.12);color:var(--accent2)}
.card{background:#fff;padding:20px;border-radius:12px;margin-top:18px;box-shadow:0 6px 18px rgba(17,24,39,0.03)}
.points{padding-left:18px;color:var(--muted)}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:12px}
.gallery{display:flex;gap:12px;margin-top:12px}
.gcell{flex:1;border-radius:8px;padding:28px;min-height:80px;background:linear-gradient(180deg,#fffef8,#fff7ed);display:flex;align-items:center;justify-content:center;color:var(--accent2);font-weight:600}
.site-footer{padding:18px 0;border-top:1px solid rgba(0,0,0,0.04);margin-top:30px;text-align:center;color:var(--muted)}
document.getElementById('year').textContent = new Date().getFullYear();
document.querySelectorAll('a[href^="#"]').forEach(a=>{
  a.addEventListener('click', e=>{
    const t = document.querySelector(a.getAttribute('href'));
    if(t){ e.preventDefault(); t.scrollIntoView({behavior:'smooth'}); }
  });
});
