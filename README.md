# Senoritaahh
🌸 Senoritaahh — Instagram Growth Landing Page  A clean, aesthetic, and responsive landing page built to promote the Instagram fitness creator **@senoritaaahh**.   This project showcases her gym lifestyle, reels, and motivational content while integrating full analytics support using **GA4**, **GTM**, and **UTM tracking**.

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Follow @senoritaaahh — Fitness & Aesthetic</title>
  <meta name="description" content="Follow senoritaaahh for gym motivation, reels and fitness tips. Visit the gallery and tap to follow." />

  <!-- ===== PLACEHOLDER FOR GTM: paste GTM <script> here (head) ===== -->
  <!-- Example: <!-- Google Tag Manager (GTM-XXXXXXX) --><script>/* GTM head snippet here */</script> -->

  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; /* dark navy */
      --card:#0b1220;
      --accent:#ff6b6b; /* coral */
      --muted:#94a3b8;
      --glass: rgba(255,255,255,0.03);
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:linear-gradient(180deg,var(--bg),#071229);color:#e6eef8;min-height:100vh}
    .container{max-width:980px;margin:36px auto;padding:20px}

    header{display:flex;align-items:center;gap:16px}
    .avatar{width:96px;height:96px;border-radius:16px;overflow:hidden;flex:0 0 96px;background:linear-gradient(135deg,#1f2937,#0f1724);display:flex;align-items:center;justify-content:center}
    .avatar img{width:100%;height:100%;object-fit:cover}
    .title{flex:1}
    .title h1{margin:0;font-size:20px;letter-spacing:0.4px}
    .title p{margin:6px 0 0;color:var(--muted);font-size:13px}

    .cta-row{display:flex;gap:12px;margin-top:18px;align-items:center}
    .btn{background:linear-gradient(90deg,var(--accent),#ff8e8e);border:none;padding:12px 18px;border-radius:12px;cursor:pointer;font-weight:600;color:#071229}
    .btn.secondary{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted)}

    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:22px}
    .card{background:var(--card);padding:8px;border-radius:12px;overflow:hidden;border:1px solid rgba(255,255,255,0.02)}
    .card img{width:100%;height:180px;object-fit:cover;border-radius:8px}
    .card .meta{padding:8px;font-size:12px;color:var(--muted)}

    .bio{margin-top:18px;background:var(--glass);padding:14px;border-radius:12px;color:var(--muted);font-size:14px}

    footer{margin-top:28px;display:flex;justify-content:space-between;align-items:center;color:var(--muted);font-size:13px}

    /* responsive */
    @media (max-width:760px){
      .grid{grid-template-columns:repeat(2,1fr)}
      header{gap:12px}
      .avatar{width:72px;height:72px}
      .card img{height:140px}
    }
    @media (max-width:420px){
      .grid{grid-template-columns:1fr}
      .cta-row{flex-direction:column;align-items:stretch}
    }

    /* small helper */
    .hidden{display:none}
  </style>
</head>
<body>
  <!-- ===== PLACEHOLDER FOR GTM (body) ===== -->
  <!-- Example: <!-- Google Tag Manager (noscript) --><noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-XXXXXXX" height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript> -->

  <main class="container">
    <header>
      <div class="avatar">
        <!-- Replace src with profile picture -->
        <img id="avatarImg" src="https://via.placeholder.com/400x400.png?text=@senoritaaahh" alt="profile" />
      </div>
      <div class="title">
        <h1 id="profileName">@senoritaaahh</h1>
        <p id="profileHandle">Fitness • Gym • Motivation</p>
        <div class="cta-row">
          <!-- MAIN FOLLOW BUTTON (opens Instagram in new tab) -->
          <button id="followBtn" class="btn">Follow on Instagram</button>
          <!-- Copy profile link -->
          <button id="copyBtn" class="btn secondary">Copy Profile Link</button>
        </div>
      </div>
    </header>

    <section class="bio" id="bioText">
      <!-- Replace with a short bio -->
      <strong>About:</strong> Gym enthusiast sharing workouts, motivation and daily fitness routines. Tap follow for daily gym inspo.
    </section>

    <section class="grid" id="mediaGrid">
      <!-- Media cards: replace images with real reel thumbnails or embed links -->
      <div class="card">
        <img src="https://picsum.photos/seed/1/800/600" alt="media 1" />
        <div class="meta">Reel • 30s • Legs Workout</div>
      </div>
      <div class="card">
        <img src="https://picsum.photos/seed/2/800/600" alt="media 2" />
        <div class="meta">Reel • 20s • Motivation</div>
      </div>
      <div class="card">
        <img src="https://picsum.photos/seed/3/800/600" alt="media 3" />
        <div class="meta">Reel • 15s • Quick Tips</div>
      </div>

      <div class="card">
        <img src="https://picsum.photos/seed/4/800/600" alt="media 4" />
        <div class="meta">Carousel • Nutrition</div>
      </div>
      <div class="card">
        <img src="https://picsum.photos/seed/5/800/600" alt="media 5" />
        <div class="meta">Reel • Transformation</div>
      </div>
      <div class="card">
        <img src="https://picsum.photos/seed/6/800/600" alt="media 6" />
        <div class="meta">Story Highlight</div>
      </div>
    </section>

    <footer>
      <div>Made with ❤️ — Organic Growth Funnel</div>
      <div id="utmNote">Share links with UTM to track sources</div>
    </footer>

    <!-- Hidden inputs to make it easy to edit the main links in the page -->
    <div class="hidden" aria-hidden="true">
      <input id="instagramUrl" type="text" value="https://www.instagram.com/senoritaaahh/" />
      <input id="profileUrlWithUtm" type="text" value="https://www.instagram.com/senoritaaahh/?utm_source=landing&utm_medium=link&utm_campaign=insta_growth" />
    </div>
  </main>

  <script>
    // Simple client-side logic for follow & copy actions
    (function(){
      const followBtn = document.getElementById('followBtn');
      const copyBtn = document.getElementById('copyBtn');
      const instagramUrlInput = document.getElementById('instagramUrl');
      const profileUrlWithUtm = document.getElementById('profileUrlWithUtm');

      // Default action: open UTM link (tracks UTM if user clicks)
      followBtn.addEventListener('click', function(){
        const url = profileUrlWithUtm.value || instagramUrlInput.value;
        // open in new tab
        window.open(url, '_blank');
        // simple analytics hook: dispatch custom event which GTM can pick up
        window.dataLayer = window.dataLayer || [];
        window.dataLayer.push({event: 'follow_click', follow_url: url});
      });

      copyBtn.addEventListener('click', async function(){
        try{
          await navigator.clipboard.writeText(instagramUrlInput.value);
          copyBtn.innerText = 'Copied!';
          setTimeout(()=> copyBtn.innerText = 'Copy Profile Link',1500);
          window.dataLayer = window.dataLayer || [];
          window.dataLayer.push({event:'copy_profile_link'});
        }catch(e){
          alert('Copy failed — open profile to copy manually');
        }
      });

      // Utility: allow quick editing by pressing E to edit links (dev-only)
      document.addEventListener('keydown', function(e){
        if(e.key.toLowerCase()==='e' && (e.ctrlKey || e.metaKey)){
          const newUrl = prompt('Set Instagram profile URL:', instagramUrlInput.value);
          if(newUrl) instagramUrlInput.value = newUrl;
          const newUtm = prompt('Set profile URL with UTM (optional):', profileUrlWithUtm.value);
          if(newUtm) profileUrlWithUtm.value = newUtm;
          alert('URLs updated. Remember to replace GTM container snippet if needed.');
        }
      });

    })();
  </script>
</body>
</html>

