# Project-Random-LeafZuya-Daffa
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fun Web by LeafZuya (Daffa)</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: linear-gradient(135deg, #4caf50, #5fe48b, #66a6ff, #3a8dde);
      color: #333;
      overflow-x: hidden;
      min-height: 100vh;
    }

    header {
      text-align: center;
      padding: 50px 20px;
      color: white;
      background: linear-gradient(135deg, rgba(0,150,136,0.7), rgba(33,150,243,0.7));
      border-bottom: 4px solid #4caf50;
      position: relative;
      overflow: hidden;
    }

    header h1 {
      font-size: 2.7rem;
      margin-bottom: 12px;
      text-shadow: 2px 2px 10px rgba(0,0,0,0.4);
    }

    header p {
      font-size: 1.2rem;
      opacity: 0.95;
    }

    /* Emoji hiasan */
    .emoji-decor {
      position: absolute;
      font-size: 2rem;
      animation: float 6s infinite ease-in-out;
    }
    .emoji1 { top: 10px; left: 20px; animation-delay: 0s; }
    .emoji2 { top: 50px; right: 20px; animation-delay: 2s; }
    .emoji3 { bottom: 15px; left: 50%; transform: translateX(-50%); animation-delay: 4s; }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    /* Container Card */
    .container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
      gap: 25px;
      padding: 50px 20px;
      max-width: 1200px;
      margin: auto;
      position: relative;
      z-index: 2;
    }

    .card {
      background: white;
      border-radius: 22px;
      padding: 22px;
      border-left: 6px solid #4caf50;
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      text-align: center;
    }

    .card:hover {
      transform: translateY(-10px) scale(1.03);
      box-shadow: 0 15px 35px rgba(0,0,0,0.25);
    }

    .card h2 {
      font-size: 1.6rem;
      margin-bottom: 12px;
      color: #2e7d32;
    }

    .card p {
      font-size: 1rem;
      color: #444;
      line-height: 1.6;
    }

    iframe {
      border-radius: 15px;
      margin: 10px;
    }

    /* Tombol */
    button {
      background: linear-gradient(135deg, #4caf50, #2196f3);
      border: none;
      padding: 12px 24px;
      border-radius: 30px;
      color: white;
      font-size: 1rem;
      font-weight: bold;
      cursor: pointer;
      transition: all 0.3s ease;
      margin-top: 10px;
    }
    button:hover {
      transform: scale(1.1);
      background: linear-gradient(135deg, #2e7d32, #1565c0);
      box-shadow: 0 8px 15px rgba(0,0,0,0.3);
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 25px;
      background: linear-gradient(135deg, rgba(0,100,0,0.6), rgba(0,70,130,0.6));
      color: white;
      margin-top: 50px;
      border-top: 4px solid #4caf50;
      font-size: 1rem;
      position: relative;
    }

    .footer-emoji {
      font-size: 1.5rem;
      margin: 0 5px;
      animation: bounce 3s infinite ease-in-out;
    }

    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-6px); }
    }

    /* Gelembung hijau-biru */
    .bubble {
      position: absolute;
      bottom: -100px;
      border-radius: 50%;
      animation: rise 12s infinite ease-in;
      z-index: 1;
    }
    .bubble.green { background: rgba(76, 175, 80, 0.5); }
    .bubble.blue { background: rgba(33, 150, 243, 0.5); }

    @keyframes rise {
      0% { transform: translateY(0) scale(1); opacity: 0.8; }
      100% { transform: translateY(-120vh) scale(1.5); opacity: 0; }
    }
  </style>
</head>
<body>
  <header>
    <h1>🌟 Welcome to My First Web 🌟</h1>
    <p>Dibuat oleh LeafZuya (Daffa) 😎🤭</p>

    <div class="emoji-decor emoji1">🍀</div>
    <div class="emoji-decor emoji2">✨</div>
    <div class="emoji-decor emoji3">💙</div>
  </header>

  <!-- Gelembung Hijau + Biru -->
  <div class="bubble green" style="left: 10%; width: 40px; height: 40px; animation-duration: 14s;"></div>
  <div class="bubble blue" style="left: 30%; width: 25px; height: 25px; animation-duration: 12s;"></div>
  <div class="bubble green" style="left: 50%; width: 50px; height: 50px; animation-duration: 16s;"></div>
  <div class="bubble blue" style="left: 70%; width: 30px; height: 30px; animation-duration: 11s;"></div>
  <div class="bubble green" style="left: 90%; width: 35px; height: 35px; animation-duration: 13s;"></div>

  <main class="container">
    <div class="card">
      <h2>✨ Tentang 🍀</h2>
      <p>Website ini dibuat cuma buat have fun aja, bukan serius. Jadi enjoyyy 😙</p>
    </div>
    <div class="card">
      <h2>📘 Pelajaran Favorit</h2>
      <p>Matematika & Informatika 💚💙 Karena Melatih Berpikir Kritis dalam menyelesaikan Sesuatu Masalah...!!!!! hehe...gak jelas ah...</p>
    </div>
    <div class="card">
      <h2>🎮 Hobi 🎶</h2>
      <p>Main game, coding iseng-iseng, dan punya mimpi jadi Indie GameDev 🥳🤞</p>
    </div>
    <div class="card">
      <h2>📺 Video Random</h2>
      <iframe width="220" height="220" src="https://www.youtube.com/embed/hyd8vfuQta0"
      title="YouTube video player" frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

      <iframe width="220" height="220" src="https://www.youtube.com/embed/nhUVc_9ki44"
      title="YouTube video player" frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
    <div class="card">
      <h2>📸 Galeri SpesialZzZz</h2>
      <iframe width="220" height="220" src="https://www.youtube.com/embed/tucpVglVsi4"
      title="YouTube video player" frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
  </main>

  <footer>
    © 2025 Fun Web by LeafZuya. Jangan Copyright...!! dan Jangan Lupa <b>BERNAFAS</b> 🤭🗣️🔥<br>
    <span class="footer-emoji">🍀</span>
    <span class="footer-emoji">💚</span>
    <span class="footer-emoji">💙</span>
  </footer>
</body>
</html>
