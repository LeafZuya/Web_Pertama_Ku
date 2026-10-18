<html lang="id">
<head>
  <!-- KODE ADSENSE DITEMPELKAN DI SINI -->
  <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-5781435134045433"
     crossorigin="anonymous"></script>
  <meta name="google-site-verification" content="df6EtL6mKtOPWlg4bi57__R4cjbLIAuNwZisuD42fHo" />
  <title>Fun Web by LeafZuya (Daffa)</title>
  <link rel="icon" type="image/png" href="favicon.png">

  <!-- 🌿 Untuk Android dan Chrome -->
  <link rel="apple-touch-icon" sizes="180x180" href="https://leafzuya.github.io/Web_Pertama_Ku/favicon.png">
  <link rel="manifest" href="https://leafzuya.github.io/Web_Pertama_Ku/manifest.json">
  <!-- 🌐 SEO Meta Tags -->
  <meta name="title" content="LeafZuya Web — Have Fun">
  <meta name="description" content="LeafZuya Adalah Website khusus untuk orang-orang yang sedang mencari kesenangan di waktu luang 🌿💙">
  <meta name="keywords" content="LeafCy, LeafZuya, AI Chat, Virtual Friend, Artificial Intelligence, Blue Archive Inspired, Web AI Indonesia, Web Have Fun, Karya Anak Gabut">
  <meta name="author" content="LeafZuya (Daffa)">

  <!-- 📱 Open Graph -->
  <meta property="og:title" content="LeafZuya Web — Have Fun">
  <meta property="og:description" content="Website ini dibuat hanya karena kegabutan LeafZuya — dan sekadar hobi di waktu luang 😆">
  <meta property="og:image" content="https://leafzuya.github.io/Web_Pertama_Ku/favicon.png">
  <meta property="og:type" content="website">
  <meta property="og:url" content="https://leafzuya.github.io/Web_Pertama_Ku/">
  <meta property="og:locale" content="id_ID">

  <!-- 🐦 Twitter Card -->
  <meta name="twitter:card" content="summary_large_image">
  <meta name="twitter:title" content="LeafZuya Web — Have Fun">
  <meta name="twitter:description" content="Website buatan LeafZuya (Daffa), dibuat hanya untuk bersenang-senang 🌿✨">
  <meta name="twitter:image" content="https://leafzuya.github.io/Web_Pertama_Ku/Favicon.png">
  <meta name="twitter:creator" content="@LeafZuya">
  
  <style>
    /* ============ LOADING SCREEN STYLES ============ */
    #loading-screen {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: linear-gradient(135deg, #1a2980, #26d0ce, #4caf50, #2e7d32);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      z-index: 9999;
      transition: opacity 1s ease, visibility 1s ease;
      font-family: 'Poppins', sans-serif;
      padding: 20px;
      text-align: center;
    }
    #loading-screen.hidden {
      opacity: 0;
      visibility: hidden;
      pointer-events: none;
    }
    #loading-title {
      color: white;
      font-size: 2.2rem;
      font-weight: 700;
      text-align: center;
      margin-bottom: 30px;
      text-shadow: 0 5px 15px rgba(0,0,0,0.3);
      animation: fadeInDown 1s ease;
      max-width: 700px;
      line-height: 1.3;
    }
    #loading-title span {
      color: #4caf50;
      text-shadow: 0 0 10px rgba(76, 175, 80, 0.5);
    }
    #start-button {
      background: linear-gradient(135deg, #ff4757, #ff3838);
      border: none;
      padding: 16px 34px;
      border-radius: 50px;
      color: white;
      font-size: 1.2rem;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 10px 30px rgba(255, 71, 87, 0.4);
      transition: all 0.3s ease;
      margin-bottom: 40px;
      animation: pulse 2s infinite;
    }
    #start-button:hover {
      transform: scale(1.07);
      box-shadow: 0 15px 40px rgba(255, 71, 87, 0.6);
    }
    @keyframes fadeInDown {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes pulse {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.05); }
    }
    #loading-container {
      display: none;
      flex-direction: column;
      align-items: center;
      width: 80%;
      max-width: 500px;
    }
    #loading-gif-container {
      width: 120px;
      height: 120px;
      margin-bottom: 25px;
      border-radius: 50%;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      background: rgba(255, 255, 255, 0.1);
      box-shadow: 0 0 30px rgba(255, 255, 255, 0.2);
    }
    #loading-gif {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      object-fit: cover;
    }
    #spinner {
      width: 80px;
      height: 80px;
      border: 6px solid rgba(255, 255, 255, 0.3);
      border-top: 6px solid #4caf50;
      border-radius: 50%;
      animation: spin 1.5s linear infinite;
      margin-bottom: 25px;
    }
    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
    #loading-progress-container {
      width: 100%;
      height: 20px;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 10px;
      overflow: hidden;
      margin-bottom: 15px;
      box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.2);
    }
    #loading-progress-bar {
      height: 100%;
      width: 0%;
      background: linear-gradient(90deg, #ff4757, #ff9f43);
      border-radius: 10px;
      transition: width 0.5s ease;
      box-shadow: 0 0 15px rgba(255, 71, 87, 0.5);
    }
    #loading-text {
      color: white;
      font-size: 1.1rem;
      font-weight: 600;
      text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
      margin-bottom: 10px;
      text-align: center;
      min-height: 30px;
    }
    #loading-percentage {
      color: #fffa65;
      font-size: 1.5rem;
      font-weight: bold;
      text-shadow: 0 2px 10px rgba(0, 0, 0, 0.4);
    }
    #audio-controls {
      margin-top: 20px;
      display: none;
      align-items: center;
      gap: 10px;
      flex-wrap: wrap;
      justify-content: center;
    }

    /* ============ STYLES UTAMA WEBSITE ============ */
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    html { scroll-behavior: smooth; }

    body {
      background: linear-gradient(135deg, #4caf50, #5fe48b, #66a6ff, #3a8dde);
      background-attachment: fixed;
      color: #333;
      overflow-x: hidden;
      min-height: 100vh;
    }
    
    .main-content {
      opacity: 0;
      transition: opacity 0.8s ease;
    }
    .main-content.loaded {
      opacity: 1;
    }

    /* ============ HEADER ============ */
    header {
      text-align: center;
      padding: 60px 20px 50px;
      color: white;
      background: linear-gradient(135deg, rgba(0,150,136,0.7), rgba(33,150,243,0.7));
      border-bottom: 4px solid #4caf50;
      position: relative;
      overflow: hidden;
    }
    header h1 {
      font-size: clamp(1.7rem, 4vw, 2.7rem);
      margin-bottom: 12px;
      text-shadow: 2px 2px 10px rgba(0,0,0,0.4);
      position: relative;
      z-index: 2;
    }
    header p {
      font-size: clamp(1rem, 2vw, 1.2rem);
      opacity: 0.95;
      position: relative;
      z-index: 2;
    }

    .emoji-decor {
      position: absolute;
      font-size: 2rem;
      animation: float 6s infinite ease-in-out;
      z-index: 1;
      opacity: 0.8;
    }
    .emoji1 { top: 10px; left: 20px; animation-delay: 0s; }
    .emoji2 { top: 50px; right: 20px; animation-delay: 2s; }
    .emoji3 { bottom: 15px; left: 50%; transform: translateX(-50%); animation-delay: 4s; }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    /* Gambar hiasan utama di header */
    .hiasan {
      display: block;
      width: 100%;
      max-width: 400px;
      height: 250px;
      object-fit: cover;
      margin: 0 auto 25px;
      border: 8px solid transparent;
      border-radius: 30px;
      background: linear-gradient(135deg, #4caf50, #2196f3);
      background-origin: border-box;
      background-clip: padding-box, border-box;
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
      position: relative;
      z-index: 2;
    }

    /* ============ GRID CONTAINER (Layout Utama) ============ */
    .container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 25px;
      padding: 50px 20px 20px;
      max-width: 1200px;
      margin: auto;
      position: relative;
      z-index: 2;
    }

    /* Card default */
    .card {
      background: white;
      border-radius: 22px;
      padding: 26px 22px;
      border-left: 6px solid #4caf50;
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      text-align: center;
      display: flex;
      flex-direction: column;
      gap: 14px;
      align-items: center;
      overflow: hidden;
    }
    .card:hover {
      transform: translateY(-8px);
      box-shadow: 0 15px 35px rgba(0,0,0,0.22);
    }
    .card h2 {
      font-size: 1.4rem;
      margin-bottom: 4px;
      color: #2e7d32;
      line-height: 1.3;
    }
    .card p {
      font-size: 0.95rem;
      color: #444;
      line-height: 1.6;
      width: 100%;
    }
    .card a {
      color: #1565c0;
      word-break: break-word;
    }

    /* Card yang melebar full-width di grid */
    .card.wide { grid-column: 1 / -1; }

    /* Gambar ilustrasi di dalam card (selain header) */
    .card .hiasan {
      max-width: 100%;
      height: auto;
      margin: 5px auto;
    }

    /* iframe */
    iframe {
      border-radius: 15px;
      border: none;
      max-width: 100%;
    }

    /* ============ TOMBOL UMUM ============ */
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
      font-family: inherit;
    }
    button:hover {
      transform: scale(1.05);
      background: linear-gradient(135deg, #2e7d32, #1565c0);
      box-shadow: 0 8px 15px rgba(0,0,0,0.3);
    }

    /* Tombol "Magic" (hijau-biru dengan kilau) — dipakai berulang di banyak card */
    .magic-btn {
      display: inline-block;
      padding: 14px 26px;
      font-size: 16px;
      font-weight: 700;
      color: white;
      text-decoration: none;
      border-radius: 18px;
      background: linear-gradient(135deg, #00e69a, #1ea7ff);
      box-shadow: 0 6px 20px rgba(0, 150, 136, 0.4);
      transition: all 0.25s ease;
      position: relative;
      overflow: hidden;
      max-width: 100%;
      line-height: 1.3;
    }
    .magic-btn::after {
      content: "";
      position: absolute;
      top: 0; left: -75%;
      width: 50%; height: 100%;
      background: rgba(255, 255, 255, 0.3);
      transform: skewX(-25deg);
      transition: all 0.6s ease;
    }
    .magic-btn:hover {
      transform: scale(1.05);
      box-shadow: 0 10px 28px rgba(0, 150, 255, 0.5);
    }
    .magic-btn:hover::after {
      left: 125%;
    }

    /* ============ JAM DIGITAL ============ */
    .jam-digital-wrapper {
      display: flex;
      justify-content: center;
      align-items: center;
      margin: 30px auto 0;
      padding: 0 20px;
      position: relative;
      z-index: 10;
    }
    .jam-digital {
      background: rgba(7, 18, 30, 0.75);
      backdrop-filter: blur(12px);
      border-radius: 60px;
      padding: 20px 40px;
      text-align: center;
      box-shadow: 
        0 0 30px rgba(0, 255, 200, 0.4),
        inset 0 0 20px rgba(0, 255, 200, 0.1),
        0 20px 30px rgba(0, 0, 0, 0.3);
      border: 1px solid rgba(0, 255, 210, 0.6);
      transition: all 0.3s ease;
      max-width: 100%;
    }
    .jam-digital:hover {
      box-shadow: 
        0 0 50px rgba(0, 255, 200, 0.7),
        inset 0 0 30px rgba(0, 255, 200, 0.2);
      transform: scale(1.02);
    }
    .waktu {
      font-size: 3.4rem;
      font-weight: 700;
      letter-spacing: 5px;
      background: linear-gradient(135deg, #0ff, #0fa);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      animation: kilauJam 1.8s infinite alternate;
    }
    .info-jam {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin-top: 10px;
      font-size: 1.3rem;
      font-weight: bold;
    }
    .detik-jam {
      color: #2af;
      text-shadow: 0 0 8px #2af, 0 0 12px #0ff;
      background: rgba(0, 255, 200, 0.15);
      padding: 4px 16px;
      border-radius: 40px;
      backdrop-filter: blur(4px);
    }
    .ampm-jam {
      color: #6f6;
      text-shadow: 0 0 8px #6f6, 0 0 12px #0f0;
      background: rgba(0, 255, 100, 0.15);
      padding: 4px 20px;
      border-radius: 40px;
      letter-spacing: 2px;
      backdrop-filter: blur(4px);
    }
    @keyframes kilauJam {
      0% { text-shadow: 0 0 5px #0ff, 0 0 10px #0ff, 0 0 20px #0af; opacity: 0.9; }
      100% { text-shadow: 0 0 15px #0ff, 0 0 30px #0ff, 0 0 60px #0ff, 0 0 90px #0fa; opacity: 1; }
    }
    @keyframes kedipJam {
      0%, 100% { opacity: 1; text-shadow: 0 0 8px #0ff; }
      50% { opacity: 0.5; text-shadow: 0 0 2px #0fa; }
    }
    .titik-jam {
      animation: kedipJam 1s infinite;
      display: inline-block;
      width: 18px;
      text-align: center;
    }
    .tanggal-jam {
      margin-top: 10px;
      font-size: 0.85rem;
      color: #8cf;
      text-shadow: 0 0 5px #0cf;
      letter-spacing: 1.5px;
      background: rgba(0, 255, 200, 0.1);
      display: inline-block;
      padding: 5px 18px;
      border-radius: 40px;
      backdrop-filter: blur(4px);
    }
    @media (max-width: 550px) {
      .jam-digital { padding: 14px 22px; }
      .waktu { font-size: 2.1rem; letter-spacing: 3px; }
      .info-jam { font-size: 1rem; gap: 12px; }
      .detik-jam, .ampm-jam { padding: 3px 12px; }
      .tanggal-jam { font-size: 0.7rem; }
      .titik-jam { width: 12px; }
    }

    /* ============ GELEMBUNG ============ */
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

    /* ============ FRAME EMAS & DONASI ============ */
    .gold-frame {
      width: 230px;
      max-width: 100%;
      border: 8px solid;
      border-image: linear-gradient(45deg, #d4af37, #f7d774, #d4af37) 1;
      padding: 8px;
      border-radius: 15px;
      background: #fff;
      box-shadow: 
        0 0 15px rgba(255, 215, 0, 0.6),
        0 0 25px rgba(255, 230, 120, 0.4);
      transition: 0.18s ease-in-out;
      cursor: pointer;
      display: inline-block;
    }
    .gold-frame:hover {
      transform: scale(1.05);
      box-shadow: 
        0 0 25px rgba(255, 215, 0, 0.9),
        0 0 40px rgba(255, 255, 150, 0.7);
    }
    .gold-frame:active { transform: scale(0.94); }
    .gold-frame img {
      width: 100%;
      border-radius: 10px;
      display: block;
    }

    .donate-btn-wrapper {
      text-align: center;
      width: 100%;
    }
    .donate-btn {
      display: inline-block;
      padding: 0;
      border-radius: 40px;
      border: 4px solid #ce1126;
      background: #000000;
      overflow: hidden;
      cursor: pointer;
      transition: 0.15s ease-in-out;
      box-shadow: 0 0 12px rgba(206, 17, 38, 0.5);
      max-width: 100%;
    }
    .donate-btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 0 18px rgba(206, 17, 38, 0.8);
    }
    .donate-btn:active {
      transform: scale(0.94);
      box-shadow: 0 0 8px rgba(206, 17, 38, 0.5);
    }
    .donate-btn img {
      width: 250px;
      max-width: 100%;
      display: block;
    }

    /* ============ FOOTER ============ */
    footer {
      text-align: center;
      padding: 28px 20px;
      background: linear-gradient(135deg, rgba(0,100,0,0.6), rgba(0,70,130,0.6));
      color: white;
      margin-top: 50px;
      border-top: 4px solid #4caf50;
      font-size: 1rem;
      position: relative;
      z-index: 2;
    }
    .footer-emoji {
      font-size: 1.5rem;
      margin: 0 5px;
      animation: bounce 3s infinite ease-in-out;
      display: inline-block;
    }
    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-6px); }
    }

    /* ============ TOMBOL "TENTANG" (Floating) ============ */
    .btn-about {
      position: fixed;
      top: 18px; right: 18px;
      background: linear-gradient(135deg, #00c16b, #27a2ff);
      color: white;
      border: none;
      border-radius: 12px;
      padding: 9px 15px;
      font-weight: 600;
      cursor: pointer;
      box-shadow: 0 4px 16px rgba(0,0,0,0.25);
      z-index: 50;
      transition: transform .2s ease, box-shadow .3s;
      font-size: 0.9rem;
    }
    .btn-about:hover {
      transform: scale(1.05);
      box-shadow: 0 0 20px rgba(255,255,150,0.5);
    }

    /* ============ HALAMAN TENTANG ============ */
    .about-page {
      position: fixed;
      inset: 0;
      background: linear-gradient(135deg, #00e69a, #39a7ff, #ffd54d33);
      display: none;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      color: #033;
      text-align: center;
      padding: 20px;
      z-index: 100;
      animation: fadeIn .6s ease;
      overflow-y: auto;
    }
    .about-page.show { display: flex; }
    .about-content {
      background: rgba(255,255,255,0.92);
      border-radius: 20px;
      box-shadow: 0 8px 50px rgba(0,0,0,0.2), 0 0 60px rgba(255,240,150,0.4);
      padding: 28px 30px;
      max-width: 620px;
      width: 100%;
      max-height: 90vh;
      overflow-y: auto;
      text-align: left;
    }
    .about-content h2 {
      color: #046;
      margin-bottom: 14px;
      text-shadow: 0 2px 10px rgba(255,255,150,0.4);
      text-align: center;
      font-size: 1.5rem;
    }
    .about-content p {
      font-size: 15px;
      line-height: 1.65;
      margin-bottom: 10px;
    }
    .about-content ul {
      list-style: none;
      padding: 0;
      margin: 15px 0;
    }
    .about-content li {
      margin: 6px 0;
      font-size: 14.5px;
    }
    .about-content h1 {
      font-size: 1.2rem;
      margin: 20px 0 10px;
      color: #046;
    }
    .dev-note {
      font-style: italic;
      font-size: 13.5px;
      margin-top: 14px;
      color: #155;
      background: rgba(0,255,200,0.08);
      padding: 10px 14px;
      border-radius: 10px;
    }
    .btn-back {
      margin-top: 20px;
      background: linear-gradient(135deg, #27a2ff, #00c16b);
      color: white;
      border: none;
      padding: 11px 20px;
      border-radius: 14px;
      cursor: pointer;
      font-weight: 600;
      transition: transform .2s ease;
      display: block;
      width: 100%;
    }
    .btn-back:hover { transform: scale(1.03); }
    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.96); }
      to { opacity: 1; transform: scale(1); }
    }

    /* ============ RESPONSIF ============ */
    @media (max-width: 640px) {
      header { padding: 50px 16px 40px; }
      .hiasan { height: 200px; }
      .container { padding: 30px 14px 10px; gap: 18px; }
      .card { padding: 22px 18px; border-radius: 18px; }
      .card h2 { font-size: 1.2rem; }
      .magic-btn { padding: 12px 20px; font-size: 14.5px; }
      iframe { width: 100% !important; height: 200px !important; }
      .donate-btn img { width: 100%; }
    }
  </style>
</head>

<body>
  <!-- ============ LOADING SCREEN ============ -->
  <div id="loading-screen">
    <h1 id="loading-title">Selamat Datang Di <span>LeafZuya Web Have Fun</span> 💚🌿</h1>
    <button id="start-button">Pencet Aku Untuk Melihat Keajaiban ✨</button>
    
    <div id="loading-container">
      <div id="loading-gif-container">
        <img id="loading-gif" src="Bah.gif" alt="Loading GIF">
      </div>
      <div id="spinner"></div>
      <div id="loading-progress-container">
        <div id="loading-progress-bar"></div>
      </div>
      <div id="loading-text">Loading pengalaman seru...</div>
      <div id="loading-percentage">0%</div>
    </div>
    
    <audio id="loading-audio" preload="auto" loop>
      <source src="Bos.mp3" type="audio/mpeg">
      Browser Anda tidak mendukung audio.
    </audio>
    
    <div id="audio-controls">
      <button id="mute-btn" style="background: rgba(255,255,255,0.2); color: white; border: 1px solid white; padding: 8px 16px; border-radius: 20px; cursor: pointer;">
        🔇 Mute
      </button>
      <input type="range" id="volume-slider" min="0" max="100" value="80" style="width: 150px; max-width: 100%;">
    </div>
  </div>
  
  <!-- ============ KONTEN UTAMA ============ -->
  <div class="main-content">
    <header>
      <img src="Iwak.gif" alt="Foto Karya" class="hiasan">
      <h1>🌟 Welcome to My First Web 🌟</h1>
      <p>Dibuat oleh LeafZuya (Daffa) 😎🤭</p>

      <div class="emoji-decor emoji1">🍀</div>
      <div class="emoji-decor emoji2">✨</div>
      <div class="emoji-decor emoji3">💙</div>
    </header>

    <!-- Jam Digital -->
    <div class="jam-digital-wrapper">
      <div class="jam-digital">
        <div class="waktu" id="jamMenitUtama">
          00<span class="titik-jam">:</span>00
        </div>
        <div class="info-jam">
          <div class="detik-jam" id="detikUtama">00</div>
          <div class="ampm-jam" id="ampmUtama">AM</div>
        </div>
        <div class="tanggal-jam" id="tanggalUtama"></div>
      </div>
    </div>

    <!-- Gelembung -->
    <div class="bubble green" style="left: 10%; width: 40px; height: 40px; animation-duration: 14s;"></div>
    <div class="bubble blue" style="left: 30%; width: 25px; height: 25px; animation-duration: 12s;"></div>
    <div class="bubble green" style="left: 50%; width: 50px; height: 50px; animation-duration: 16s;"></div>
    <div class="bubble blue" style="left: 70%; width: 30px; height: 30px; animation-duration: 11s;"></div>
    <div class="bubble green" style="left: 90%; width: 35px; height: 35px; animation-duration: 13s;"></div>

    <main class="container">
      <!-- Card Tentang -->
      <div class="card">
        <h2>✨ Tentang 🍀</h2>
        <p>Website ini dibuat cuma buat have fun aja, bukan serius. Jadi enjoyyy 😙</p>
        <p>Kirim kritik dan saran kalian ke <a href="mailto: kingglafeon@gmail.com">Gmail Ku [LeafZuya(Daffa)]....hehehe...🥳</a></p>

        <div style="margin: 12px 0;">
          <a href="https://trakteer.id/leafzuya%28daffa%29" target="_blank" style="text-decoration:none;">
            <button style="
              background: linear-gradient(135deg, #ff4e50, #f9d423);
              border: none;
              padding: 14px 28px;
              border-radius: 40px;
              color: white;
              font-size: 1rem;
              font-weight: bold;
              cursor: pointer;
              box-shadow: 0 5px 15px rgba(0,0,0,0.2);
              transition: all 0.3s ease;">
              🍵 Bagi yang mau Traktir......buat Beli Laptop ♥️🥳
            </button>
          </a>
        </div>

        <button onclick="playMusic('Jokowi.mp3')">Jangan Pencet Aku....☠️🗿</button>
        <audio id="audio1" src="Jokowi.mp3"></audio>
        <button onclick="playMusic('gok.mp3')">Jangan Pencet Aku....☠️🗿v2</button>
        <audio id="audio2" src="gok.mp3"></audio>

        <p><b>JANGAN COBA-COBA SCREENSHOOT CODE QR DIBAWAH INI,LALU MEMINDAI NYA DI PEMINDAI QR CODE 🗿☠️💀</b></p>
        <img src="Idiot.jpg" alt="Gambar Karya" width="200" height="200" style="border-radius:12px;">
      </div>

      <!-- Card Quiz Kemerdekaan -->
      <div class="card" style="
        border: 3px solid #000;
        background: linear-gradient(135deg, #d90000, #ffffff, #ff0202, #e3b1b1);
        color: #000;
      ">
        <h2 style="text-align:center; color:#000; font-weight:bold;">
          🇮🇩QUIZ SPESIAL HARI KEMERDEKAAN (Limited Event)🔥
        </h2>

        <div>
          <div class="gold-frame" onclick="playFrameSound()">
            <img src="Merdeka.png" alt="Support Palestine">
          </div>
          <audio id="frameSound" src="IDN.mp3"></audio>
        </div>

        <div class="donate-btn-wrapper">
          <a href="Miami.html" target="_blank" class="donate-btn">
            <img src="MerdekaT.png" alt="Donasi Palestina">
          </a>
        </div>

        <p style="text-align:center; background:#ff5c5c; padding:12px; border-radius:10px;">
          <b>"🇮🇩 'Bangsaku yang tercinta, janganlah kamu lupa pada sejarah perjuanganmu. Karena dari sanalah kita belajar untuk terus maju.'"</b><br>
          <b>~By:LeafZuya</b>
        </p>
        <p style="text-align:center; background:#ffffff; padding:12px; border-radius:10px;">Gass Aja Mainin,bakal Di Tutup saat <b>25 Agustus 2026</b> Awokawokawok</p>
      </div>

      <!-- Card Donasi Palestina -->
      <div class="card" style="
        border: 3px solid #000;
        background: linear-gradient(135deg, #1a1a1a, #ffffff, #009739, #ce1126);
        color: #000;
      ">
        <h2 style="text-align:center; color:#000; font-weight:bold;">
          🇵🇸 Donasi Untuk Palestina
        </h2>

        <div>
          <div class="gold-frame" onclick="playFrameSound2()">
            <img src="Palestina.jpg" alt="Support Palestine">
          </div>
          <audio id="frameSound2" src="Free.mp3"></audio>
        </div>

        <div class="donate-btn-wrapper">
          <a href="https://www.rumahzakat.org/donasi/palestina" target="_blank" class="donate-btn">
            <img src="PalestinaT.jpg" alt="Donasi Palestina">
          </a>
        </div>

        <p style="text-align:center; background:#fff; padding:12px; border-radius:10px;">
          Bantu saudara-saudara kita di Palestina yang sedang mengalami krisis kemanusiaan.  
          Sepeser Bantuan kecil dari kalian dapat memberi dampak besar bagi mereka.  
          🇵🇸💚 Terima kasih untuk kebaikan hati kalian.<br>
          <b>~By:LeafZuya</b>
        </p>
        <p style="text-align:center; background:#fff; padding:12px; border-radius:10px;">Nanti Kalian Akan Diarahkan Ke <b>WEBSITE/SITUS RESMI DAN AMAN</b> untuk Menyumbangkan Amal Sumbangan...Jadi Uang-Nya Tidak Masuk Ke <b>REKENING PRIBADI-KU</b> Yahh!!...</p>
      </div>

      <!-- Card Pelajaran -->
      <div class="card">
        <h2>📘 Pelajaran Favorit</h2>
        <p>Matematika & Informatika 💚💙 Karena Melatih Berpikir Kritis dalam menyelesaikan Sesuatu Masalah...!!!!! hehe...gak jelas ah...</p>
      </div>

      <!-- Card Hobi -->
      <div class="card">
        <h2>🎮 Hobi 🎶</h2>
        <p>Main game, coding iseng-iseng, dan punya mimpi jadi Indie GameDev 🥳🤞</p>
      </div>

      <!-- Card Video Random -->
      <div class="card">
        <h2>📺 Video Random</h2>
        <iframe width="100%" height="220" src="https://www.youtube.com/embed/hyd8vfuQta0"
          title="YouTube video player" frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <iframe width="100%" height="220" src="https://www.youtube.com/embed/nhUVc_9ki44"
          title="YouTube video player" frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>

      <!-- Card Karya Danang -->
      <div class="card">
        <h2>Penasaran Karya Danang...?, Klik Dibawah Ini ya...!😋</h2>
        <p><a href="https://leafzuya.github.io/Khusus_Danang/">Klik aku untuk melihat berbagai Karya Buatan Danang.....😆</a></p>
        <p>Jangan Lupa Follow Akun Media Sosialnya...!!</p>
        <p><a href="https://tiktok.com/@zainaki_and_hoshino">Media Sosial Danang</a></p>
      </div>

      <!-- TIC TAC TOE -->
      <div class="card" id="ttt-card">
        <h2>🎯 Tic-Tac-Toe — Player vs AI</h2>
        <p>Pilih sisi & tingkat kesulitan, lalu kalahkan AI kalau bisa 😎</p>

        <div id="ttt-controls" style="display:flex; gap:10px; flex-wrap:wrap; justify-content:center; margin-bottom:12px;">
          <label> Kamu main:
            <select id="ttt-side" style="padding:6px 10px; border-radius:10px; border:1px solid #9acdff;">
              <option value="X">❌ X</option>
              <option value="O">⭕ O</option>
            </select>
          </label>
          <label> Kesulitan:
            <select id="ttt-difficulty" style="padding:6px 10px; border-radius:10px; border:1px solid #9acdff;">
              <option value="easy">Easy</option>
              <option value="medium">Medium</option>
              <option value="hard">Hard</option>
              <option value="impossible" selected>Impossible 😈</option>
            </select>
          </label>
          <button id="ttt-new">🔁 New</button>
          <button id="ttt-undo">↩️ Undo</button>
          <button id="ttt-hint">💡 Hint</button>
        </div>

        <div id="ttt-board"
             style="--cell:88px; margin:0 auto; display:grid; grid-template-columns:repeat(3,1fr); gap:10px; width:fit-content;">
        </div>

        <div id="ttt-status" style="margin-top:14px; font-weight:600; color:#2e7d32;">Status: siap!</div>
        <div id="ttt-score" style="margin-top:6px; opacity:.9;">Skor — Kamu: <span id="s-you">0</span> | AI: <span id="s-ai">0</span> | Seri: <span id="s-draw">0</span></div>

        <style>
          #ttt-board .ttt-cell{
            height:var(--cell); width:var(--cell); display:flex; align-items:center; justify-content:center;
            font-size:calc(var(--cell)*.55); font-weight:700; cursor:pointer; user-select:none;
            border-radius:16px;
            background:linear-gradient(145deg,#e8fff0,#f7fbff);
            box-shadow: 0 8px 18px rgba(0,0,0,.12), inset 0 0 0 2px rgba(76,175,80,.18);
            transition: transform .12s ease, box-shadow .2s ease, background .2s ease;
          }
          #ttt-board .ttt-cell:hover{ transform:translateY(-2px); box-shadow:0 12px 22px rgba(0,0,0,.18), inset 0 0 0 2px rgba(33,150,243,.18);}
          #ttt-board .ttt-cell.played{ animation: pop .12s ease-out; }
          #ttt-board .ttt-cell.win{ background:linear-gradient(145deg,#b2fab4,#b3e5fc) !important; box-shadow:0 0 0 3px rgba(76,175,80,.6) inset, 0 8px 22px rgba(0,0,0,.18);}
          #ttt-board .ttt-cell.disabled{ pointer-events:none; opacity:.7; }
          @keyframes pop { from{transform:scale(.85);} to{transform:scale(1);} }

          #ttt-card button{
            background: linear-gradient(135deg, #4caf50, #2196f3);
            border: none; padding: 10px 16px; border-radius: 24px; color: #fff;
            font-weight:700; cursor:pointer; box-shadow: 0 8px 15px rgba(0,0,0,.2); transition: transform .15s ease, box-shadow .2s ease;
            font-size: 0.9rem;
          }
          #ttt-card button:hover{ transform: translateY(-2px); box-shadow:0 12px 22px rgba(0,0,0,.25);}
          #ttt-card select{ background:#fff; }
          @media (max-width:420px){
            #ttt-board{ --cell:78px; gap:8px; }
          }
        </style>

        <script>
        (function(){
          const boardEl = document.getElementById('ttt-board');
          const statusEl = document.getElementById('ttt-status');
          const sYou = document.getElementById('s-you'), sAi = document.getElementById('s-ai'), sDraw = document.getElementById('s-draw');
          const selSide = document.getElementById('ttt-side');
          const selDiff = document.getElementById('ttt-difficulty');
          const btnNew = document.getElementById('ttt-new'), btnUndo = document.getElementById('ttt-undo'), btnHint = document.getElementById('ttt-hint');

          let board, human, ai, turn, finished, history, scores = {you:0, ai:0, draw:0};
          const lines = [[0,1,2],[3,4,5],[6,7,8],[0,3,6],[1,4,7],[2,5,8],[0,4,8],[2,4,6]];
          const TT = new Map();

          const cells = [];
          for (let i=0;i<9;i++){
            const c = document.createElement('div');
            c.className = 'ttt-cell';
            c.dataset.idx = i;
            c.addEventListener('click', () => humanMove(i));
            boardEl.appendChild(c);
            cells.push(c);
          }

          function reset(){
            board = Array(9).fill(null);
            human = selSide.value; ai = (human==='X'?'O':'X');
            turn = 'X';
            finished = false;
            history = [];
            cells.forEach(c => { c.textContent=''; c.classList.remove('played','win','disabled'); });
            setStatus("Giliran: " + glyph(turn));
            maybeAiFirst();
          }
          function glyph(p){ return p==='X'?'❌ X':'⭕ O'; }
          function maybeAiFirst(){ if (turn === ai){ setTimeout(()=> aiMove(), 250); } }
          function setStatus(t){ statusEl.textContent = "Status: " + t; }
          function humanMove(i){
            if (finished || turn!==human || board[i]) return;
            pushHistory(); place(i, human); afterMove();
          }
          function aiMove(){
            if (finished || turn!==ai) return;
            const diff = selDiff.value;
            let move;
            if (diff === 'easy') move = randomMove();
            else if (diff === 'medium') move = bestMove({maxDepth:2, jitter:true});
            else if (diff === 'hard') move = bestMove({maxDepth:6});
            else move = bestMove({maxDepth:9});
            pushHistory(); place(move, ai, true); afterMove();
          }
          function randomMove(){
            const avail = board.map((v,idx)=> v?null:idx).filter(v=>v!==null);
            return avail[Math.floor(Math.random()*avail.length)];
          }
          function afterMove(){
            const res = winner(board);
            if (res){ endGame(res); return; }
            turn = (turn==='X'?'O':'X');
            setStatus("Giliran: " + glyph(turn));
            if (turn===ai) setTimeout(()=> aiMove(), 220);
          }
          function place(i, who, isAi=false){
            board[i] = who;
            const cell = cells[i];
            cell.textContent = (who==='X'?'X':'O');
            cell.style.color = (who==='X'?'#2e7d32':'#1565c0');
            cell.classList.add('played');
          }
          function winner(b){
            for (const [a,b1,c] of lines){
              if (b[a] && b[a]===b[b1] && b[a]===b[c]) return {win:b[a], line:[a,b1,c]};
            }
            if (b.every(v=>v)) return {draw:true};
            return null;
          }
          function endGame(res){
            finished = true;
            cells.forEach(c=> c.classList.add('disabled'));
            if (res.draw){
              setStatus("Seri 🤝");
              scores.draw++; sDraw.textContent = scores.draw;
            } else {
              const isHumanWin = (res.win === human);
              res.line.forEach(i=> cells[i].classList.add('win'));
              if (isHumanWin){ setStatus("Kamu MENANG! 🏆"); scores.you++; sYou.textContent = scores.you; }
              else { setStatus("AI menang 😈"); scores.ai++; sAi.textContent = scores.ai; }
            }
          }
          function pushHistory(){ history.push({board:[...board], turn, finished}); }
          function undo(){
            if (!history.length) return;
            const prev = history.pop();
            board = prev.board; turn = prev.turn; finished = prev.finished;
            cells.forEach((c,i)=> {
              c.textContent = board[i]||'';
              c.classList.remove('win','disabled','played');
              if (board[i]) c.classList.add('played');
            });
            setStatus("Undo. Giliran: " + glyph(turn));
          }
          function hint(){
            if (finished || board.every(v=>v)) return;
            const move = (turn===ai) ? bestMove({maxDepth: selDiff.value==='impossible'?9:6})
                                     : (selDiff.value==='easy'?randomMove():bestMove({maxDepth:4, jitter:true}));
            if (move==null) return;
            cells[move].style.boxShadow = "0 0 0 3px rgba(33,150,243,.7) inset, 0 12px 22px rgba(0,0,0,.2)";
            setTimeout(()=> cells[move].style.boxShadow='', 650);
          }
          function bestMove({maxDepth=9, jitter=false}={}){
            const me = ai, opp = human;
            const order = [4,0,2,6,8,1,3,5,7].filter(i=>!board[i]);
            let best = null, bestScore = -Infinity;
            for (const m of order){
              board[m]=turn;
              const sc = -negamax(board, switchTurn(turn), 1, -Infinity, Infinity, maxDepth, me, opp);
              board[m]=null;
              if (sc > bestScore || (jitter && sc===bestScore && Math.random()<.3)){
                bestScore = sc; best = m;
              }
            }
            return best;
          }
          function negamax(b, toMove, depth, alpha, beta, me, opp){
            const w = winner(b);
            if (w){
              if (w.draw) return 0;
              const val = (w.win===me) ? (10 - depth) : (depth - 10);
              return val;
            }
            if (depth>=9) return 0;
            const key = hash(b, toMove);
            const tt = TT.get(key);
            if (tt && tt.depth >= depth) return tt.score;
            const moves = [4,0,2,6,8,1,3,5,7].filter(i=>!b[i]);
            let best = -Infinity;
            for (const m of moves){
              b[m]=toMove;
              const score = -negamax(b, switchTurn(toMove), depth+1, -beta, -alpha, me, opp);
              b[m]=null;
              if (score>best) best=score;
              if (best>alpha) alpha=best;
              if (alpha>=beta) break;
            }
            TT.set(key,{score:best, depth});
            return best;
          }
          function switchTurn(t){ return t==='X'?'O':'X'; }
          function hash(b, t){ return (b.map(v=>v||'-').join('') + t); }

          btnNew.addEventListener('click', reset);
          btnUndo.addEventListener('click', undo);
          btnHint.addEventListener('click', hint);
          selSide.addEventListener('change', reset);
          selDiff.addEventListener('change', reset);
          reset();
        })();
        </script>
      </div>

      <!-- Card Tangkap Emoji -->
      <div class="card">
        <h2>Tangkap Emoji....!!😎🥳😵</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="Emoji.jpg" alt="Foto Karya" class="hiasan">
        <p><a href="https://leafzuya.github.io/Web-Have-Fun-/">Klik aku untuk Mainkan...!!!,Kalo kalah, Berarti Noob😎☝️</a></p>
        <p>Cara mainnya tinggal di Klik ke kanan atau ke kiri aja,lalu tangkap semua dan kumpulkan point sebanyak-banyaknya.....!!!(Hanya disediakan 3 Nyawa/Kesempatan)</p>
      </div>

      <!-- Card Sound Memory -->
      <div class="card">
        <h2>Sound Memory....!!🗣️🎤🎧</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="Simon.jpg" alt="Foto Karya" class="hiasan">
        <p><a href="https://leafzuya.github.io/Sound-Memori-/">Klik aku untuk Mainkan sound memori...!!!,Kalo cepat kalah, Berarti jangan main ini lagi,main sana game Roblox 🤓☝️</a></p>
        <p>Cara mainnya tinggal ikuti irama yang muncul acak dan pencet tombol sesuai irama yang muncul pada tombol tersebut.....semakin lama akan semakin banyak irama yang akan di putar/mainkan..... Semangat....!!!🥳♥️🔥</p>
      </div>

      <!-- Card Kalkulator -->
      <div class="card">
        <h2>Kalkulator LeafZuya 😆🌿➗➖➕</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="Kalkulator.jpg" alt="Foto Karya" class="hiasan">
        <p><a href="https://leafzuya.github.io/Kalkulator-/">Klik aku untuk Menjalankan Kalkulator,versi Buatan ku sendiri.....</a></p>
        <p>Konon katanya,orang yang menggunakan Kalkulator Ini,bisa menambahkan IQ Manusia Maksimal sampai 105....🗿👍</p>
      </div>

      <!-- Card LeafCy AI -->
      <div class="card">
        <h2>LeafCy AI😆🌿</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="leafcy.png" alt="Foto Karya" class="hiasan">
        <a href="https://leafcyai.my.id/" class="magic-btn">Kunjungi LeafCy AI☘️😆</a>
        <p>Jangan Lupa Klik Tombol Diatas yah....Itu adalah AI Buatan ku Sendiri (LeafZuya),tapi masih Tahap Pengembangan (Beta)...kalian juga bisa Tambahkan Obrolan dan Jawaban Obrolan Nya...[LeafCy AI X OpenRouter]😆🤞☘️🍃</p>
      </div>

      <!-- Card Leaf-Wheel -->
      <div class="card">
        <h2>Leaf-Wheel🎡🌿</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="Wheel.jpg" alt="Foto Karya" class="hiasan">
        <a href="https://leafzuya.github.io/Leaf_Wheel/" class="magic-btn">Kunjungi Leaf-Wheel☘️🎡</a>
        <p>Butuh Roda Penentu Keberuntungan???, Cobain Leaf-Wheel Yukkk!!!!🗿🙏☘️🎡</p>
      </div>

      <!-- Card Cek Hewan -->
      <div class="card">
        <h2>Cek Hewan Dalam Jiwa Kalian!!🌿</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="Hewan.jpg" alt="Foto Karya" class="hiasan">
        <a href="https://leafzuya.github.io/Cek-Hewan-/" class="magic-btn">Kunjungi Cek Hewan Dalam Jiwa ☘️✅🗿</a>
        <p>Apakah Kalian Sering Bertanya Dalam Hati"Sebenarnya, Apasih Hewan/Khodam Dalam Diri ku ini?"...Nahh,untuk itu, Kunjungi Minigame Diatas,untuk Memecahkan Rasa Penasaran Kamu...🗿🙏☕</p>
      </div>

      <!-- Card LeafPy -->
      <div class="card">
        <h2>LeafPy!🐦🌿</h2>
        <p><b>Dibawah ini Hanya Gambar Ilustrasi saja!!</b></p>
        <img src="LeafPy.jpg" alt="Foto Karya" class="hiasan">
        <a href="https://leafzuya.github.io/LeafPy/" class="magic-btn">Game Burung Santai, selamat Bermain  ☕🗿🍃🐦</a>
        <p>Kalian Suka Tantangan Skor Paling Banyak Dengan Orang lain Di Seluruh Dunia???,Nahhh...kalian Datang Di tempat yang Tepat,Di LeafPy,Kalian Bisa Mengumpulkan Skor sebanyak-banyaknya dengan cara melewati Rintangan Pipa Merah!!!, Minigame Ini juga Dilengkapi Leaderboard Online Mengandalkan Server Storage Browser....(Butuh Waktu 4 Minggu Woilah Baru Selesai 🗿🙏☕)</p>
      </div>

      <!-- Card LeafFast -->
      <div class="card">
        <h2>Uji Kekuatan Kecepatan Jari!🌿</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="Fast.jpg" alt="Foto Karya" class="hiasan">
        <a href="https://leafzuya.github.io/LeafFast/" class="magic-btn">Kunjungi LeafFast ☘️✅🗿</a>
        <p>Apakah Kalian Mempunyai Kekuatan Kecepatan Super???,Kalo iya,buktikan Dengan Memainkan Minigame ini🗿🙏☕</p>
      </div>

      <!-- Card Leaf Flip -->
      <div class="card">
        <h2>Uji Ingatan Otak!🌿</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="Flip.png" alt="Foto Karya" class="hiasan">
        <a href="https://leafzuya.github.io/Leaf_Flip/" class="magic-btn">Mainkan Supaya Punya IQ tinggi!☘️🗿</a>
        <p>Ingin Punya Ingatan Super???,Ingin Punya IQ Tingi???,Nahh...Mainkan Lah,Minigame Ini!🗿🙏☕</p>
      </div>

      <!-- Card Sneaky -->
      <div class="card">
        <h2>Sneaky!🌿🗿</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="Sneak.jpg" alt="Foto Karya" class="hiasan">
        <a href="https://leafzuya.github.io/Sneaky/" class="magic-btn">Mainkan Sneaky! ☘️🗿</a>
        <p>Game Gabut Final Bos,Tema Nostalgia+Jadul,tapi Dengan Nuansa Dan Fitur Modern!🗿🙏☕</p>
      </div>

      <!-- Card ReflexZ -->
      <div class="card">
        <h2>ReflexZ😆🌿</h2>
        <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
        <img src="ReflexZ.png" alt="Foto Karya" class="hiasan">
        <a href="ReflexZ.html" class="magic-btn">Kunjungi ReflexZ!😆</a>
        <p>Gas Aja Mainin,ga Usah Basa-Basi🤞🍃</p>
      </div>

      <!-- Tombol Tentang -->
      <button id="aboutBtn" class="btn-about">ℹ️ Tentang(Opsional,tapi Disarankan 🗿☕)</button>

      <!-- Halaman Tentang -->
      <section id="aboutPage" class="about-page">
        <div class="about-content">
          <h2>🌿 LeafZuya Web Have Fun</h2>
          <p>
            Website ini dibuat sebagai hiburan Di Waktu Luang,Jangan Terlalu Fokus/Serius pada Website ini,Hidup kalian lebih berwarna,jika kalian melakukan Hal-Hal yang Bermanfaat untuk Orang lain dan Diri Sendiri...Ingat!,kita Ini Makhluk Yang Lemah!,Jangan Sombong kepada sang Pencipta!,Karena Dialah yang Berkuasa atas Dunia Ini,dan Jangan Lupa <b>BERBUAT BAIK</b> 💚.
          </p>
          <p>Website Ini Dipercayai Oleh 150+ Orang² Gabut dari Seluruh Dunia,dan Diawasi Oleh Organisasi Perkumpulan Orang² Gabut Se-Asia Tenggara(OPO2GAT)</p>

          <ul>
            <li>Dibuat Sejak:10 Agustus 2025</li>
            <li><b>🧩 Versi:</b> v17.8.45— "Blood Leaves of Struggle🇮🇩🔥"</li>
            <li><b>💬 Dibuat oleh:</b> <span style="color:#09b;">LeafZuya(Daffa)</span></li>
            <li><b>📅 Update terakhir:</b> 16 Agustus 2026</li>
          </ul>

          <p class="dev-note">
            ✨ Catatan Developer:<br>
            "Ubahlah Waktu Luang Kalian Yang Tidak Bermanfaat,Menjadi <b>SEDIKIT</b> lebih Bermanfaat"
          </p>

          <h1>•Apa Yang Baru?</h1>
          <p>-Memperbaiki Bug</p>
          <p>-Mengubah Deskripsi dan Gambar Ilustrasi LeafCy AI</p>
          <p>-Update LeafCy AI,Jadi Punya Logikanya Sendiri!!😆</p>
          <p>-Update LeafCy Jadi Punya Akselerasi buat Mengetik "Zuya Ganteng 😎 " Sebanyak 1000x,Untuk Me-Redeem Pengurangan Waktu Selama 30 Menit🗿🙏</p>

          <button id="backBtn" class="btn-back">⬅️ Kembali</button>
        </div>
      </section>
    </main>

    <footer>
      © 2025 Fun Web by LeafZuya. Jangan Copyright...!! dan Jangan Lupa 
      <b>BERNAFAS</b> 🤭🗣️🔥<br>
      <span class="footer-emoji">🍀</span>
      <span class="footer-emoji">💚</span>
      <span class="footer-emoji">💙</span>
    </footer>
  </div>

  <!-- ============ SCRIPT GLOBAL (audio card + frame) ============ -->
  <script>
    function playMusic(soundFile) {
      let audio;
      if (soundFile === 'Jokowi.mp3') {
        audio = document.getElementById("audio1");
      } else {
        audio = document.getElementById("audio2");
      }
      audio.currentTime = 0;
      audio.play();
    }
    function playFrameSound() {
      const audio = document.getElementById("frameSound");
      audio.currentTime = 0;
      audio.play();
    }
    function playFrameSound2() {
      const audio = document.getElementById("frameSound2");
      audio.currentTime = 0;
      audio.play();
    }
  </script>

  <!-- ============ SCRIPT LOADING SCREEN ============ -->
  <script>
  document.addEventListener('DOMContentLoaded', function() {
    const loadingScreen = document.getElementById('loading-screen');
    const startButton = document.getElementById('start-button');
    const loadingContainer = document.getElementById('loading-container');
    const progressBar = document.getElementById('loading-progress-bar');
    const loadingPercentage = document.getElementById('loading-percentage');
    const loadingAudio = document.getElementById('loading-audio');
    const mainContent = document.querySelector('.main-content');
    const loadingText = document.getElementById('loading-text');
    const muteBtn = document.getElementById('mute-btn');
    const volumeSlider = document.getElementById('volume-slider');
    const audioControls = document.getElementById('audio-controls');
    
    const customGifUrl = '';
    const loadingGif = document.getElementById('loading-gif');
    
    if (customGifUrl) {
      loadingGif.src = customGifUrl;
    } else {
      document.getElementById('loading-gif-container').style.display = 'none';
    }
    
    if (loadingAudio) {
      loadingAudio.loop = true;
      loadingAudio.volume = volumeSlider.value / 100;
      setTimeout(() => { audioControls.style.display = 'flex'; }, 1000);
    }
    
    window.changeLoadingMusic = function(newUrl) {
      if (loadingAudio) {
        loadingAudio.pause();
        loadingAudio.src = newUrl;
        loadingAudio.load();
        setTimeout(() => { playAudioWithInteraction(); }, 500);
      }
    };
    
    function playAudioWithInteraction() {
      if (!loadingAudio) return;
      const playPromise = loadingAudio.play();
      if (playPromise !== undefined) {
        playPromise.then(() => {
          console.log("Audio berhasil diputar otomatis");
        }).catch(error => {
          console.log("Auto-play dicegah:", error);
          loadingText.textContent = "Klik tombol 'Start' untuk memutar musik...";
          startButton.addEventListener('click', function playOnInteraction() {
            loadingAudio.play().then(() => {
              startButton.removeEventListener('click', playOnInteraction);
            });
          }, { once: true });
        });
      }
    }
    
    if (volumeSlider && loadingAudio) {
      volumeSlider.addEventListener('input', function() {
        loadingAudio.volume = this.value / 100;
        muteBtn.innerHTML = (this.value == 0) ? '🔇 Mute' : '🔊 Unmute';
      });
    }
    
    if (muteBtn && loadingAudio) {
      muteBtn.addEventListener('click', function() {
        if (loadingAudio.muted) {
          loadingAudio.muted = false;
          this.innerHTML = '🔊 Unmute';
        } else {
          loadingAudio.muted = true;
          this.innerHTML = '🔇 Mute';
        }
      });
    }
    
    function startLoading() {
      startButton.style.display = 'none';
      loadingContainer.style.display = 'flex';
      playAudioWithInteraction();
      
      let progress = 0;
      const totalDuration = 9000;
      const intervalDuration = 100;
      const progressPerInterval = 100 / (totalDuration / intervalDuration);
      const messages = [
        "Menyiapkan pengalaman seru...",
        "Memuat konten menarik...",
        "Menyiapkan game-game keren...",
        "Hampir selesai...",
        "Selamat Datang & Selamat Bersenang-Senang!(•LeafZuya•)"
      ];
      let messageIndex = 0;
      
      const interval = setInterval(() => {
        progress += progressPerInterval;
        if (progress > 100) progress = 100;
        progressBar.style.width = progress + '%';
        loadingPercentage.textContent = Math.floor(progress) + '%';
        
        if (progress < 20 && messageIndex < 1) { loadingText.textContent = messages[0]; messageIndex = 1; }
        else if (progress >= 20 && progress < 40 && messageIndex < 2) { loadingText.textContent = messages[1]; messageIndex = 2; }
        else if (progress >= 40 && progress < 60 && messageIndex < 3) { loadingText.textContent = messages[2]; messageIndex = 3; }
        else if (progress >= 60 && progress < 80 && messageIndex < 4) { loadingText.textContent = messages[3]; messageIndex = 4; }
        else if (progress >= 80 && messageIndex < 5) { loadingText.textContent = messages[4]; messageIndex = 5; }
        
        if (Math.floor(progress) === 50 && loadingAudio) {
          const currentVol = loadingAudio.volume;
          if (currentVol < 0.9) loadingAudio.volume = currentVol * 1.2;
        }
        
        if (progress >= 100) {
          clearInterval(interval);
          if (loadingAudio) {
            const fadeAudio = setInterval(() => {
              if (loadingAudio.volume > 0.1) {
                loadingAudio.volume -= 0.05;
              } else {
                loadingAudio.pause();
                loadingAudio.currentTime = 0;
                loadingAudio.volume = volumeSlider.value / 100;
                clearInterval(fadeAudio);
              }
            }, 50);
          }
          setTimeout(() => {
            loadingScreen.classList.add('hidden');
            mainContent.classList.add('loaded');
            audioControls.style.display = 'none';
          }, 800);
        }
      }, intervalDuration);
    }
    
    startButton.addEventListener('click', startLoading);
    
    setTimeout(() => {
      if (startButton.style.display !== 'none') {
        playAudioWithInteraction();
        loadingText.textContent = "Memulai otomatis dalam 3 detik...";
        setTimeout(startLoading, 3000);
      }
    }, 10000);
    
    window.changeMusic = function(url) {
      if (loadingAudio) {
        loadingAudio.pause();
        loadingAudio.src = url;
        loadingAudio.load();
        loadingAudio.play().catch(e => console.log("Gagal memutar:", e));
        console.log("Musik loading screen telah diganti!");
      }
    };
  });
  </script>

  <!-- ============ SCRIPT JAM DIGITAL ============ -->
  <script>
  function updateJamDigital() {
    const now = new Date();
    let jam24 = now.getHours();
    const menit = now.getMinutes().toString().padStart(2, '0');
    const detik = now.getSeconds().toString().padStart(2, '0');
    const ampm = jam24 >= 12 ? 'PM' : 'AM';
    const jamFormatted = jam24.toString().padStart(2, '0');

    const jamMenitElem = document.getElementById('jamMenitUtama');
    if (jamMenitElem) jamMenitElem.innerHTML = `${jamFormatted}<span class="titik-jam">:</span>${menit}`;
    
    const detikElem = document.getElementById('detikUtama');
    if (detikElem) detikElem.innerText = detik;
    
    const ampmElem = document.getElementById('ampmUtama');
    if (ampmElem) ampmElem.innerText = ampm;

    const options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' };
    const tanggalString = now.toLocaleDateString('id-ID', options);
    const tanggalElem = document.getElementById('tanggalUtama');
    if (tanggalElem) tanggalElem.innerHTML = '📅 ' + tanggalString;
  }
  updateJamDigital();
  setInterval(updateJamDigital, 1000);
  </script>

  <!-- ============ SCRIPT TOMBOL TENTANG ============ -->
  <script>
  const aboutBtn = document.getElementById('aboutBtn');
  const aboutPage = document.getElementById('aboutPage');
  const backBtn = document.getElementById('backBtn');

  aboutBtn.addEventListener('click', ()=>{ aboutPage.classList.add('show'); });
  backBtn.addEventListener('click', ()=>{ aboutPage.classList.remove('show'); });
  </script>
</body>
</html>
