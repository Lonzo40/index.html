# index.html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Jeanette & Alonso — Love Portfolio</title>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg1: #fff7fb;
      --bg2: #f0f9ff;
      --accent1: #ff6b9a;
      --accent2: #6bd6ff;
      --muted: #6b6b6b;
      --card: rgba(255,255,255,0.85);
      --glass: rgba(255,255,255,0.6);
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial}
    body{background:linear-gradient(160deg,var(--bg1),var(--bg2));color:#111;line-height:1.45}
    header{display:flex;align-items:center;justify-content:space-between;padding:18px 24px;max-width:1100px;margin:0 auto}
    .logo{display:flex;gap:12px;align-items:center}
    .logo .mark{width:56px;height:56px;border-radius:14px;background:linear-gradient(135deg,var(--accent1),var(--accent2));display:flex;align-items:center;justify-content:center;color:white;font-weight:800;font-family:Playfair Display,serif}
    nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:600}
    .hero{max-width:1100px;margin:18px auto;padding:28px;border-radius:18px;background:linear-gradient(180deg,rgba(255,255,255,0.8),rgba(255,255,255,0.6));box-shadow:0 8px 30px rgba(60,60,80,0.08);display:grid;grid-template-columns:1fr 420px;gap:22px;align-items:center}
    .intro h1{font-family:Playfair Display,serif;font-size:36px;margin:0 0 8px}
    .intro p{color:var(--muted);margin:0 0 18px}
    .cta{display:flex;gap:10px}
    .btn{padding:10px 16px;border-radius:12px;border:0;font-weight:700;cursor:pointer}
    .btn-primary{background:linear-gradient(90deg,var(--accent1),#ff8bbd);color:white}
    .btn-ghost{background:transparent;border:1px solid rgba(0,0,0,0.06)}
    .portrait{display:flex;flex-direction:column;align-items:center;gap:12px}
    .portrait img{width:92%;border-radius:14px;box-shadow:0 10px 30px rgba(50,50,80,0.08)}
    .names{display:flex;gap:10px;font-weight:700;color:#333}
    .names span{background:var(--card);padding:8px 12px;border-radius:999px}
    .sections{max-width:1100px;margin:26px auto;display:grid;grid-template-columns:repeat(3,1fr);gap:18px;padding:0 18px}
    .card{background:var(--card);padding:18px;border-radius:14px;backdrop-filter:blur(6px);box-shadow:0 6px 22px rgba(30,30,60,0.05)}
    .card h3{margin:0 0 8px;font-size:18px}
    .card p{margin:0;color:var(--muted);font-size:14px}
    .gallery{max-width:1100px;margin:24px auto;padding:18px;display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
    .gallery img{width:100%;height:180px;object-fit:cover;border-radius:12px}
    .music{max-width:1100px;margin:24px auto;padding:18px;display:flex;gap:18px;align-items:center;justify-content:space-between}
    .music .note{color:var(--muted)}
    footer{max-width:1100px;margin:36px auto;padding:18px;color:var(--muted);display:flex;justify-content:space-between}
    @media (max-width:980px){.hero{grid-template-columns:1fr;padding:18px}.sections{grid-template-columns:repeat(1,1fr)}.gallery{grid-template-columns:repeat(2,1fr)}}
    @media (max-width:520px){nav{display:none}.gallery{grid-template-columns:1fr}.intro h1{font-size:26px}}
    .decor-heart{position:fixed;right:14px;bottom:14px;background:linear-gradient(180deg,var(--accent1),var(--accent2));width:52px;height:52px;border-radius:50%;display:flex;align-items:center;justify-content:center;color:white;font-weight:800;box-shadow:0 10px 30px rgba(120,80,120,0.08)}
  </style>
</head>
<body>
  <header>
    <div class="logo">
      <div class="mark">J&A</div>
      <div>
        <div style="font-weight:700">Jeanette & Alonso</div>
        <small style="color:var(--muted)">Adventures • Love • Life</small>
      </div>
    </div>
    <nav>
      <a href="#about">About</a>
      <a href="#gallery">Gallery</a>
      <a href="#music">Music</a>
    </nav>
  </header>

  <main>
    <section class="hero" aria-labelledby="hero-heading">
      <div class="intro">
        <h1 id="hero-heading">Two hummingbirds, one story</h1>
        <p>Welcome to our little corner of the internet  a colorful, minimal tribute to the moments that shaped us. Save this page, add the music, and come back whenever you need a reminder of how far we've come.</p>
        <div class="cta">
          <button class="btn btn-primary" onclick="document.getElementById('about').scrollIntoView({behavior:'smooth'})">Our Story</button>
          <button class="btn btn-ghost" onclick="document.getElementById('music').scrollIntoView({behavior:'smooth'})">Play Music</button>
        </div>
        <div style="margin-top:18px;color:var(--muted);font-size:14px">Tip: On mobile, tap the music control to start playback (autoplay may be blocked by some browsers).</div>
      </div>

      <aside class="portrait" aria-label="Jeanette and Alonso portrait">
        <!-- Mobile-ready hero image -->
        <img src="hummingbirds.JPG" alt="Two hummingbirds photo">
        <div class="names">
          <span>Jeanette</span>
          <span>Alonso</span>
        </div>
      </aside>
    </section>

    <section id="about" class="sections" aria-labelledby="about-heading">
      <div class="card">
        <h3 id="about-heading">Adventures</h3>
        <p>From sunrise hikes to midnight drives — we collect memories. This section holds snapshots and short notes about the places we've been and the ones we dream of.</p>
      </div>
      <div class="card">
        <h3>Love</h3>
        <p>Small gestures, big meaning. Love here is a practice — patience, laughter, shared playlists, and the rituals that make us us.</p>
      </div>
      <div class="card">
        <h3>Life</h3>
        <p>Everyday life — routines and surprises. This is the glue: home projects, cooking experiments, and growing together.</p>
      </div>
    </section>

    <section id="gallery" class="gallery" aria-label="Gallery">
      <img src="gallery1.jpg" alt="Gallery photo 1">
      <img src="gallery2.jpg" alt="Gallery photo 2">
      <img src="gallery3.jpg" alt="Gallery photo 3">
    </section>

    <section id="music" class="music" aria-labelledby="music-heading">
      <div>
        <h3 id="music-heading">Our Song</h3>
        <p class="note">Tap play to hear the song — replace with your own audio if needed.</p>
      </div>
      <div>
        <audio id="player" controls loop>
          <source src="song.mp3" type="audio/mpeg">
          Your browser does not support the audio element.
        </audio>
      </div>
    </section>
  </main>

  <footer>
    <div>Built with ♥</div>
    <div style="font-size:13px;color:var(--muted)">Made for Jeanette & Alonso — replace images & text freely</div>
  </footer>

  <div class="decor-heart" title="Love">❤</div>

  <script>
    document.addEventListener('keydown', (e)=>{
      if(e.key === 'm' || e.key === 'M'){
        const p = document.getElementById('player');
        if(p){ if(p.paused) p.play().catch(()=>{}); else p.pause(); }
      }
    });
    window.addEventListener('load', ()=>{
      const p = document.getElementById('player');
      if(p && window.innerWidth > 520){
        p.play().catch(()=>{});
      }
    });
  </script>
</body>
</html>
