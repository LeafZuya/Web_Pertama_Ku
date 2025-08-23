# Project-gabut-Daffa-LeafZuya
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fun Web by LeafZuya(Daffa)</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: linear-gradient(120deg, #89f7fe, #66a6ff, #5fe48b);
      color: #333;
      overflow-x: hidden;
    }

    header {
      text-align: center;
      padding: 40px 20px;
      color: white;
      background: linear-gradient(135deg, rgba(0,0,0,0.3), rgba(0,100,0,0.5));
      backdrop-filter: blur(6px);
      border-bottom: 4px solid #4caf50;
      position: relative;
    }

    header h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.3);
    }

    header p {
      font-size: 1.2rem;
      opacity: 0.9;
    }

    /* ✨ Dekorasi emoji di header */
    .emoji-decor {
      position: absolute;
      font-size: 2rem;
      animation: float 6s infinite ease-in-out;
    }

    .emoji1 { top: 10px; left: 20px; animation-delay: 0s; }
    .emoji2 { top: 50px; right: 20px; animation-delay: 2s; }
    .emoji3 { bottom: 10px; left: 50%; transform: translateX(-50%); animation-delay: 4s; }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    .container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
      padding: 40px;
      max-width: 1200px;
      margin: auto;
      position: relative;
      z-index: 2;
    }

    .card {
      background: white;
      border-radius: 20px;
      padding: 20px;
      border-left: 6px solid #4caf50;
      box-shadow: 0 8px 20px rgba(0,0,0,0.15);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      text-align: center;
      position: relative;
    }

    .card:hover {
      transform: translateY(-10px) scale(1.03);
      box-shadow: 0 12px 30px rgba(0,0,0,0.25);
    }

    .card h2 {
      font-size: 1.5rem;
      margin-bottom: 10px;
      color: #2e7d32;
    }

    .card p {
      font-size: 1rem;
      color: #444;
      line-height: 1.6;
    }

    /* 🎨 Style tombol */
    button {
      background: linear-gradient(135deg, #4caf50, #66bb6a);
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
      background: linear-gradient(135deg, #2e7d32, #4caf50);
      box-shadow: 0 8px 15px rgba(0,0,0,0.2);
    }

    footer {
      text-align: center;
      padding: 20px;
      background: linear-gradient(135deg, rgba(0,0,0,0.4), rgba(0,100,0,0.6));
      color: white;
      margin-top: 40px;
      backdrop-filter: blur(4px);
      border-top: 4px solid #4caf50;
      font-size: 1rem;
      position: relative;
    }

    /* 🌟 Dekorasi Gelembung Hijau */
    .bubble {
      position: absolute;
      bottom: -100px;
      width: 40px;
      height: 40px;
      background: rgba(76, 175, 80, 0.5);
      border-radius: 50%;
      animation: rise 10s infinite ease-in;
    }

    @keyframes rise {
      0% { transform: translateY(0) scale(1); opacity: 0.8; }
      100% { transform: translateY(-120vh) scale(1.5); opacity: 0; }
    }

    /* 🍀 Emoji dekor di footer */
    .footer-emoji {
      font-size: 1.5rem;
      margin: 0 5px;
      animation: bounce 3s infinite ease-in-out;
    }

    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-6px); }
    }
  </style>
</head>
<body>
  <header>
    <h1>🌟 Welcome to My First Web 🌟</h1>
    <p>Dibuat oleh LeafZuya(Daffa)😎🤫</p>

    <!-- Emoji dekorasi -->
    <div class="emoji-decor emoji1">🍀</div>
    <div class="emoji-decor emoji2">✨</div>
    <div class="emoji-decor emoji3">💚</div>
  </header>

  <!-- Gelembung Hijau -->
  <div class="bubble" style="left: 10%; animation-duration: 12s;"></div>
  <div class="bubble" style="left: 30%; animation-duration: 15s; width: 25px; height: 25px;"></div>
  <div class="bubble" style="left: 50%; animation-duration: 9s; width: 50px; height: 50px;"></div>
  <div class="bubble" style="left: 70%; animation-duration: 14s;"></div>
  <div class="bubble" style="left: 90%; animation-duration: 11s; width: 30px; height: 30px;"></div>

  <main class="container">
    <div class="card">
      <h2>✨ Tentang 🍀</h2>
      <p>Ini website have fun, bukan serius. Jadi enjoy aja yaa~ 😙</p>
    </div>
    <div class="card">
      <h2>📘 Pelajaran Favorit?</h2>
      <p>Tentunya Matematika dan Informatika...!!💚💚 Pelajaran yang melatih Berpikir Kritis dalam menyelesaikan masalah..! wkwkwkw gak jelas ah...</p>
    </div>
    <div class="card">
      <h2>🎮 Hobi 🎶</h2>
      <p>Main game, belajar coding iseng-iseng, dan memiliki mimpi untuk menjadi GameDev Indie😙🤞</p>
    </div>
    <div class="card">
      <h2>📺 "Video Random Kesukaanku..."</h2>
       <iframe width="200" height="200"
  src="https://www.youtube.com/embed/hyd8vfuQta0?autoplay=1"
  title="YouTube video player"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen></iframe>

      <iframe width="200" height="200"
  src="https://www.youtube.com/embed/nhUVc_9ki44"
  title="USSR anthem Indonesian and russian sub"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen></iframe>

       <h2>⚠️ Bila Video Tidak Bisa Diputar</h2>
       <p>1. Buka Pengaturan Browser di pojok kanan atas<br></p>
       <p>2. Pencet "Mode Desktop" di pengaturan (tidak peduli nyala/mati)<br></p>
       <p>3. Jika muncul "Halaman Tidak Diketahui / about:blank", pencet tombol "Back" pada handphone<br></p>
    </div>
  </main>

     <div class="card">
  <h2>📸 Galeri SpesialZzZz</h2>

<iframe width="200" height="200"
  src="https://www.youtube.com/embed/tucpVglVsi4"
  title="YouTube video player" frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  allowfullscreen>
</iframe>
  
</div>

  <footer>
    © 2025 Fun Web by LeafZuya. Tidak Boleh Copyright.<br>
    jangan lupa <b>BERNAFAS</b> 🤫🗣️ Ang Ang Ang😛<br>
    <span class="footer-emoji">🍀</span>
    <span class="footer-emoji">💚</span>
    <span class="footer-emoji">🌿</span>
  </footer>
</body>
</html>
