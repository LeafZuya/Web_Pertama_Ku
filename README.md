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

  <!-- 📱 Open Graph (Facebook, Discord, Google Rich Preview) -->
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

  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    /* ============ GOOGLE FONTS ============ */
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap');

    /* ============ ROOT VARIABLES (TEMA WARNA ASLI DIPERTAHANKAN) ============ */
    :root {
      --grad-main: linear-gradient(135deg, #4caf50, #5fe48b, #66a6ff, #3a8dde);
      --grad-header: linear-gradient(135deg, rgba(0,150,136,0.85), rgba(33,150,243,0.85));
      --grad-btn: linear-gradient(135deg, #4caf50, #2196f3);
      --grad-btn-hover: linear-gradient(135deg, #2e7d32, #1565c0);
      --grad-footer: linear-gradient(135deg, rgba(0,100,0,0.85), rgba(0,70,130,0.85));
      --grad-accent: linear-gradient(135deg, #00e69a, #1ea7ff);
      --green: #4caf50;
      --green-dark: #2e7d32;
      --blue: #2196f3;
      --blue-dark: #1565c0;
      --text: #333;
      --text-light: #666;
      --surface: rgba(255,255,255,0.92);
      --surface-solid: #ffffff;
      --card-border: rgba(76,175,80,0.25);
      --shadow-soft: 0 10px 30px rgba(0,0,0,0.10);
      --shadow-hover: 0 18px 45px rgba(0,0,0,0.18);
      --sidebar-bg: rgba(255,255,255,0.85);
      --sidebar-text: #2e7d32;
      --radius-lg: 22px;
      --radius-md: 16px;
      --radius-sm: 12px;
      --transition: 0.3s cubic-bezier(.25,.8,.25,1);
    }

    /* DARK MODE */
    body.dark-mode {
      --text: #e8f5e9;
      --text-light: #b0bec5;
      --surface: rgba(28,38,45,0.92);
      --surface-solid: #1c262d;
      --card-border: rgba(76,175,80,0.35);
      --sidebar-bg: rgba(24,33,39,0.92);
      --sidebar-text: #a5d6a7;
      --shadow-soft: 0 10px 30px rgba(0,0,0,0.4);
      --shadow-hover: 0 18px 45px rgba(0,0,0,0.55);
      background: #10181d;
    }

    /* ============ GLOBAL RESET ============ */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    html { scroll-behavior: smooth; }

    body {
      background: var(--grad-main);
      background-attachment: fixed;
      color: var(--text);
      overflow-x: hidden;
      min-height: 100vh;
      transition: background 0.5s ease, color 0.4s ease;
    }

    body.dark-mode {
      background: linear-gradient(135deg, #0b1418, #12232b, #0f1b2e, #0a1420);
      background-attachment: fixed;
    }

    /* ============ LOADING SCREEN ============ */
    #loading-screen {
      position: fixed;
      inset: 0;
      background: var(--grad-main);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      z-index: 9999;
      transition: opacity 1s ease, visibility 1s ease;
      padding: 20px;
    }

    #loading-screen.hidden {
      opacity: 0;
      visibility: hidden;
      pointer-events: none;
    }

    #loading-title {
      color: white;
      font-size: clamp(1.5rem, 4vw, 2.5rem);
      font-weight: 700;
      text-align: center;
      margin-bottom: 30px;
      text-shadow: 0 5px 15px rgba(0,0,0,0.3);
      animation: fadeInDown 1s ease;
      line-height: 1.4;
    }

    #loading-title span {
      color: #eaffea;
      text-shadow: 0 0 15px rgba(76, 175, 80, 0.7);
    }

    #start-button {
      background: linear-gradient(135deg, #ff4757, #ff3838);
      border: none;
      padding: 18px 36px;
      border-radius: 50px;
      color: white;
      font-size: clamp(1rem, 2.5vw, 1.3rem);
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 10px 30px rgba(255, 71, 87, 0.4);
      transition: all 0.3s ease;
      margin-bottom: 40px;
      animation: pulse 2s infinite;
    }

    #start-button:hover {
      transform: scale(1.08);
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

    #loading-gif { width: 100px; height: 100px; border-radius: 50%; object-fit: cover; }

    #spinner {
      width: 80px; height: 80px;
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
      width: 100%; height: 20px;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 10px;
      overflow: hidden;
      margin-bottom: 15px;
      box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.2);
    }

    #loading-progress-bar {
      height: 100%; width: 0%;
      background: linear-gradient(90deg, #ff4757, #ff9f43);
      border-radius: 10px;
      transition: width 0.5s ease;
      box-shadow: 0 0 15px rgba(255, 71, 87, 0.5);
    }

    #loading-text {
      color: white; font-size: 1.1rem; font-weight: 600;
      text-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
      margin-bottom: 10px; text-align: center; min-height: 30px;
    }

    #loading-percentage {
      color: #fffa65; font-size: 1.5rem; font-weight: bold;
      text-shadow: 0 2px 10px rgba(0, 0, 0, 0.4);
    }

    /* ============ MAIN LAYOUT ============ */
    .main-content {
      opacity: 0;
      transition: opacity 0.8s ease;
      min-height: 100vh;
    }

    .main-content.loaded { opacity: 1; }

    .app-layout {
      display: flex;
      min-height: 100vh;
    }

    /* ============ SIDEBAR ============ */
    .sidebar {
      position: fixed;
      top: 0; left: 0;
      width: 270px;
      height: 100vh;
      background: var(--sidebar-bg);
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      border-right: 1px solid rgba(76,175,80,0.2);
      display: flex;
      flex-direction: column;
      padding: 24px 16px;
      z-index: 1000;
      transition: transform var(--transition), background 0.4s ease;
      overflow-y: auto;
      box-shadow: 4px 0 25px rgba(0,0,0,0.08);
    }

    .sidebar::-webkit-scrollbar { width: 6px; }
    .sidebar::-webkit-scrollbar-thumb { background: rgba(76,175,80,0.4); border-radius: 3px; }

    .sidebar-brand {
      display: flex;
      align-items: center;
      gap: 12px;
      padding: 0 8px 20px;
      border-bottom: 1px solid rgba(76,175,80,0.2);
      margin-bottom: 18px;
    }

    .sidebar-brand .brand-logo {
      width: 44px; height: 44px;
      border-radius: 14px;
      background: var(--grad-accent);
      display: flex; align-items: center; justify-content: center;
      font-size: 1.4rem;
      box-shadow: 0 6px 18px rgba(0, 200, 150, 0.35);
      flex-shrink: 0;
    }

    .sidebar-brand .brand-text h3 {
      font-size: 1.05rem; font-weight: 700;
      color: var(--sidebar-text);
      line-height: 1.2;
    }

    .sidebar-brand .brand-text p {
      font-size: 0.72rem;
      color: var(--text-light);
      font-weight: 500;
    }

    .sidebar-nav {
      display: flex;
      flex-direction: column;
      gap: 4px;
      flex: 1;
    }

    .nav-section-label {
      font-size: 0.68rem;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      font-weight: 700;
      color: var(--text-light);
      padding: 14px 12px 6px;
      opacity: 0.7;
    }

    .nav-item {
      display: flex;
      align-items: center;
      gap: 12px;
      padding: 11px 14px;
      border-radius: var(--radius-sm);
      color: var(--text);
      text-decoration: none;
      font-size: 0.9rem;
      font-weight: 500;
      cursor: pointer;
      transition: background 0.2s ease, transform 0.2s ease, color 0.2s ease;
      border: none;
      background: transparent;
      width: 100%;
      text-align: left;
    }

    .nav-item .nav-icon {
      font-size: 1.15rem;
      width: 24px;
      text-align: center;
      flex-shrink: 0;
    }

    .nav-item:hover {
      background: linear-gradient(135deg, rgba(76,175,80,0.12), rgba(33,150,243,0.12));
      transform: translateX(4px);
      color: var(--green-dark);
    }

    body.dark-mode .nav-item:hover { color: #a5d6a7; }

    .nav-item.active {
      background: var(--grad-btn);
      color: white;
      box-shadow: 0 6px 18px rgba(76,175,80,0.35);
    }

    .sidebar-footer {
      padding-top: 16px;
      border-top: 1px solid rgba(76,175,80,0.2);
      margin-top: 12px;
    }

    .theme-toggle-btn {
      display: flex;
      align-items: center;
      gap: 12px;
      width: 100%;
      padding: 12px 14px;
      border-radius: var(--radius-sm);
      border: 1px solid rgba(76,175,80,0.3);
      background: rgba(76,175,80,0.08);
      color: var(--text);
      font-weight: 600;
      font-size: 0.9rem;
      cursor: pointer;
      transition: all 0.25s ease;
    }

    .theme-toggle-btn:hover {
      background: rgba(76,175,80,0.18);
      transform: translateY(-1px);
    }

    /* ============ CONTENT AREA ============ */
    .content-area {
      flex: 1;
      margin-left: 270px;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
      transition: margin-left var(--transition);
    }

    /* ============ TOP BAR ============ */
    .topbar {
      position: sticky;
      top: 0;
      z-index: 900;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
      padding: 14px 28px;
      background: var(--surface);
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      border-bottom: 1px solid rgba(76,175,80,0.15);
      box-shadow: 0 2px 20px rgba(0,0,0,0.06);
    }

    .menu-toggle-btn {
      display: none;
      background: var(--grad-btn);
      border: none;
      width: 42px; height: 42px;
      border-radius: 12px;
      color: white;
      font-size: 1.3rem;
      cursor: pointer;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 14px rgba(76,175,80,0.35);
      transition: transform 0.2s ease;
    }

    .menu-toggle-btn:hover { transform: scale(1.06); }

    .topbar-title {
      font-size: 1.15rem;
      font-weight: 700;
      color: var(--text);
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .topbar-title span { color: var(--green); }

    .topbar-actions {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .topbar-icon-btn {
      width: 42px; height: 42px;
      border-radius: 12px;
      border: 1px solid rgba(76,175,80,0.25);
      background: var(--surface-solid);
      color: var(--text);
      font-size: 1.15rem;
      cursor: pointer;
      display: flex; align-items: center; justify-content: center;
      transition: all 0.22s ease;
    }

    .topbar-icon-btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 6px 16px rgba(76,175,80,0.25);
      border-color: var(--green);
    }

    /* ============ HERO HEADER ============ */
    .hero {
      position: relative;
      text-align: center;
      padding: 60px 28px 50px;
      color: white;
      background: var(--grad-header);
      border-bottom: 4px solid var(--green);
      overflow: hidden;
    }

    .hero .hiasan {
      width: min(400px, 85%);
      height: 250px;
      object-fit: cover;
      border: 8px solid transparent;
      border-radius: 30px;
      background: linear-gradient(135deg, #4caf50, #2196f3);
      padding: 5px;
      box-shadow: 0 12px 35px rgba(0,0,0,0.35);
      margin-bottom: 22px;
      position: relative;
      z-index: 2;
    }

    .hero h1 {
      font-size: clamp(1.6rem, 4vw, 2.7rem);
      margin-bottom: 12px;
      text-shadow: 2px 2px 10px rgba(0,0,0,0.4);
      position: relative;
      z-index: 2;
    }

    .hero p {
      font-size: clamp(1rem, 2.2vw, 1.2rem);
      opacity: 0.95;
      position: relative;
      z-index: 2;
    }

    .emoji-decor {
      position: absolute;
      font-size: 2rem;
      animation: float 6s infinite ease-in-out;
      z-index: 1;
      opacity: 0.9;
    }
    .emoji1 { top: 20px; left: 8%; animation-delay: 0s; }
    .emoji2 { top: 60px; right: 8%; animation-delay: 2s; }
    .emoji3 { bottom: 20px; left: 50%; transform: translateX(-50%); animation-delay: 4s; }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    /* ============ JAM DIGITAL ============ */
    .jam-digital-wrapper {
      display: flex;
      justify-content: center;
      align-items: center;
      margin: 28px auto 10px auto;
      padding: 0 20px;
      position: relative;
      z-index: 10;
    }

    .jam-digital {
      background: rgba(7, 18, 30, 0.78);
      backdrop-filter: blur(12px);
      border-radius: 60px;
      padding: 20px 40px;
      text-align: center;
      box-shadow: 0 0 30px rgba(0, 255, 200, 0.4), inset 0 0 20px rgba(0, 255, 200, 0.1), 0 20px 30px rgba(0, 0, 0, 0.3);
      border: 1px solid rgba(0, 255, 210, 0.6);
      transition: all 0.3s ease;
      max-width: 100%;
    }

    .jam-digital:hover {
      box-shadow: 0 0 50px rgba(0, 255, 200, 0.7), inset 0 0 30px rgba(0, 255, 200, 0.2);
      transform: scale(1.02);
    }

    .waktu {
      font-size: 3.8rem;
      font-weight: 700;
      letter-spacing: 6px;
      background: linear-gradient(135deg, #0ff, #0fa);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      animation: kilauJam 1.8s infinite alternate;
      line-height: 1.1;
    }

    .info-jam {
      display: flex;
      justify-content: center;
      gap: 25px;
      margin-top: 12px;
      font-size: 1.4rem;
      font-weight: bold;
    }

    .detik-jam {
      color: #2af;
      text-shadow: 0 0 8px #2af, 0 0 12px #0ff;
      background: rgba(0, 255, 200, 0.15);
      padding: 5px 18px;
      border-radius: 40px;
      backdrop-filter: blur(4px);
    }

    .ampm-jam {
      color: #6f6;
      text-shadow: 0 0 8px #6f6, 0 0 12px #0f0;
      background: rgba(0, 255, 100, 0.15);
      padding: 5px 22px;
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

    .titik-jam { animation: kedipJam 1s infinite; display: inline-block; width: 18px; text-align: center; }

    .tanggal-jam {
      margin-top: 12px;
      font-size: 0.9rem;
      color: #8cf;
      text-shadow: 0 0 5px #0cf;
      letter-spacing: 1.5px;
      background: rgba(0, 255, 200, 0.1);
      display: inline-block;
      padding: 5px 20px;
      border-radius: 40px;
      backdrop-filter: blur(4px);
    }

    @media (max-width: 550px) {
      .jam-digital { padding: 12px 20px; }
      .waktu { font-size: 2.2rem; letter-spacing: 3px; }
      .info-jam { font-size: 1rem; gap: 12px; }
      .detik-jam, .ampm-jam { padding: 3px 12px; }
      .tanggal-jam { font-size: 0.7rem; }
      .titik-jam { width: 12px; }
    }

    /* ============ BUBBLES ============ */
    .bubble {
      position: fixed;
      bottom: -100px;
      border-radius: 50%;
      animation: rise 12s infinite ease-in;
      z-index: 0;
      pointer-events: none;
    }
    .bubble.green { background: rgba(76, 175, 80, 0.4); }
    .bubble.blue { background: rgba(33, 150, 243, 0.4); }

    @keyframes rise {
      0% { transform: translateY(0) scale(1); opacity: 0.8; }
      100% { transform: translateY(-120vh) scale(1.5); opacity: 0; }
    }

    /* ============ MAIN SECTION ============ */
    main.container {
      padding: 40px 28px 20px;
      max-width: 1300px;
      margin: 0 auto;
      width: 100%;
      position: relative;
      z-index: 2;
      flex: 1;
    }

    /* MASONRY LAYOUT */
    .cards-masonry {
      column-count: 3;
      column-gap: 22px;
    }

    @media (max-width: 1100px) { .cards-masonry { column-count: 2; } }
    @media (max-width: 700px)  { .cards-masonry { column-count: 1; } }

    /* ============ CARD ============ */
    .card {
      display: inline-block;
      width: 100%;
      margin: 0 0 22px;
      background: var(--surface);
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
      border-radius: var(--radius-lg);
      padding: 24px;
      border: 1px solid var(--card-border);
      border-left: 5px solid var(--green);
      box-shadow: var(--shadow-soft);
      transition: transform var(--transition), box-shadow var(--transition), background 0.4s ease;
      text-align: center;
      overflow: hidden;
      break-inside: avoid;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: var(--shadow-hover);
    }

    .card h2 {
      font-size: 1.3rem;
      margin-bottom: 14px;
      color: var(--green-dark);
      line-height: 1.35;
      font-weight: 700;
    }

    body.dark-mode .card h2 { color: #a5d6a7; }

    .card p {
      font-size: 0.94rem;
      color: var(--text-light);
      line-height: 1.65;
      margin-bottom: 8px;
    }

    .card a {
      color: var(--blue-dark);
      font-weight: 600;
      text-decoration: none;
      transition: color 0.2s ease;
      word-break: break-word;
    }
    .card a:hover { text-decoration: underline; color: var(--green-dark); }
    body.dark-mode .card a { color: #64b5f6; }
    body.dark-mode .card a:hover { color: #a5d6a7; }

    .card iframe {
      border-radius: var(--radius-md);
      margin: 8px;
      max-width: 100%;
    }

    .hiasan {
      width: min(400px, 100%);
      height: 250px;
      object-fit: cover;
      border: 8px solid transparent;
      border-radius: 30px;
      background: linear-gradient(135deg, #4caf50, #2196f3);
      padding: 5px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
      margin: 10px auto;
      display: block;
    }

    /* ============ BUTTONS ============ */
    button {
      background: var(--grad-btn);
      border: none;
      padding: 12px 24px;
      border-radius: 30px;
      color: white;
      font-size: 0.95rem;
      font-weight: 700;
      cursor: pointer;
      transition: all 0.3s ease;
      margin-top: 10px;
      font-family: inherit;
    }
    button:hover {
      transform: translateY(-2px) scale(1.03);
      background: var(--grad-btn-hover);
      box-shadow: 0 8px 15px rgba(0,0,0,0.3);
    }

    /* ============ GOLD FRAME ============ */
    .gold-frame {
      width: min(230px, 100%);
      border: 8px solid;
      border-image: linear-gradient(45deg, #d4af37, #f7d774, #d4af37) 1;
      padding: 8px;
      border-radius: 15px;
      background: #fff;
      box-shadow: 0 0 15px rgba(255, 215, 0, 0.6), 0 0 25px rgba(255, 230, 120, 0.4);
      transition: 0.18s ease-in-out;
      cursor: pointer;
      margin: 0 auto;
    }
    .gold-frame:hover { transform: scale(1.05); box-shadow: 0 0 25px rgba(255, 215, 0, 0.9), 0 0 40px rgba(255, 255, 150, 0.7); }
    .gold-frame:active { transform: scale(0.94); }
    .gold-frame img { width: 100%; border-radius: 10px; display: block; }

    /* ============ DONATE BTN ============ */
    .donate-btn-wrapper { text-align: center; margin: 10px 0; }
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
    .donate-btn:hover { transform: translateY(-2px); box-shadow: 0 0 18px rgba(206, 17, 38, 0.8); }
    .donate-btn:active { transform: scale(0.94); }
    .donate-btn img { width: min(250px, 100%); display: block; }

    /* ============ MAGIC BUTTON ============ */
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
      margin: 10px 0;
      max-width: 100%;
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
    .magic-btn:hover { transform: scale(1.05); box-shadow: 0 10px 28px rgba(0, 150, 255, 0.5); text-decoration: none; color: white; }
    .magic-btn:hover::after { left: 125%; }

    /* ============ TIC TAC TOE ============ */
    #ttt-board .ttt-cell {
      height: var(--cell);
      aspect-ratio: 1/1;
      display: flex; align-items: center; justify-content: center;
      font-size: calc(var(--cell) * 0.55);
      font-weight: 700;
      cursor: pointer;
      user-select: none;
      border-radius: 16px;
      background: linear-gradient(145deg, #e8fff0, #f7fbff);
      box-shadow: 0 8px 18px rgba(0,0,0,.12), inset 0 0 0 2px rgba(76,175,80,.18);
      transition: transform .12s ease, box-shadow .2s ease, background .2s ease;
    }
    body.dark-mode #ttt-board .ttt-cell {
      background: linear-gradient(145deg, #243b30, #1a2b38);
    }
    #ttt-board .ttt-cell:hover { transform: translateY(-2px); box-shadow: 0 12px 22px rgba(0,0,0,.18), inset 0 0 0 2px rgba(33,150,243,.18); }
    #ttt-board .ttt-cell.played { animation: pop .12s ease-out; }
    #ttt-board .ttt-cell.win { background: linear-gradient(145deg,#b2fab4,#b3e5fc) !important; box-shadow: 0 0 0 3px rgba(76,175,80,.6) inset, 0 8px 22px rgba(0,0,0,.18); }
    #ttt-board .ttt-cell.disabled { pointer-events: none; opacity: .7; }
    @keyframes pop { from{transform:scale(.85);} to{transform:scale(1);} }

    #ttt-card button {
      background: var(--grad-btn);
      border: none; padding: 10px 16px; border-radius: 24px; color: #fff;
      font-weight: 700; cursor: pointer;
      box-shadow: 0 8px 15px rgba(0,0,0,.2);
      transition: transform .15s ease, box-shadow .2s ease;
    }
    #ttt-card button:hover { transform: translateY(-2px); box-shadow: 0 12px 22px rgba(0,0,0,.25); }
    #ttt-card select { background: var(--surface-solid); color: var(--text); }
    @media (max-width: 420px) { #ttt-board { --cell: 86px; gap: 8px; width: calc(var(--cell)*3); } }
    @media (max-width: 360px) { #ttt-board { --cell: 78px; gap: 8px; width: calc(var(--cell)*3); } }

    /* ============ ABOUT PAGE ============ */
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
      z-index: 2000;
      animation: fadeIn .6s ease;
      overflow-y: auto;
    }
    .about-page.show { display: flex; }

    .about-content {
      background: rgba(255,255,255,0.94);
      border-radius: 20px;
      box-shadow: 0 8px 50px rgba(0,0,0,0.2), 0 0 60px rgba(255,240,150,0.4);
      padding: 26px 30px;
      max-width: 600px;
      width: 90%;
      margin: auto;
      text-align: left;
    }
    .about-content h2 { color: #046; margin-bottom: 12px; text-shadow: 0 2px 10px rgba(255,255,150,0.4); }
    .about-content p { font-size: 15px; line-height: 1.6; margin-bottom: 10px; color: #033; }
    .about-content ul { text-align: left; list-style: none; padding: 0; margin: 15px 0; }
    .about-content li { margin: 6px 0; font-size: 14.5px; color: #033; }
    .about-content h1 { font-size: 1.3rem; margin: 14px 0 8px; color: #046; }
    .dev-note { font-style: italic; font-size: 13.5px; margin-top: 14px; color: #155; }

    .btn-about {
      position: fixed;
      top: 18px; right: 18px;
      background: linear-gradient(135deg, #00c16b, #27a2ff);
      color: white;
      border: none;
      border-radius: 12px;
      padding: 8px 14px;
      font-weight: 600;
      cursor: pointer;
      box-shadow: 0 4px 16px rgba(0,0,0,0.25);
      z-index: 50;
      transition: transform .2s ease, box-shadow .3s;
    }
    .btn-about:hover { transform: scale(1.05); box-shadow: 0 0 20px rgba(255,255,150,0.5); }

    .btn-back {
      margin-top: 20px;
      background: linear-gradient(135deg, #27a2ff, #00c16b);
      color: white;
      border: none;
      padding: 10px 18px;
      border-radius: 14px;
      cursor: pointer;
      font-weight: 600;
      transition: transform .2s ease;
    }
    .btn-back:hover { transform: scale(1.05); }

    @keyframes fadeIn {
      from { opacity: 0; transform: scale(0.96); }
      to { opacity: 1; transform: scale(1); }
    }

    /* ============ FOOTER ============ */
    footer {
      text-align: center;
      padding: 28px 20px;
      background: var(--grad-footer);
      color: white;
      margin-top: 40px;
      border-top: 4px solid var(--green);
      font-size: 0.95rem;
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

    /* ============ OVERLAY (mobile sidebar) ============ */
    .sidebar-overlay {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.5);
      backdrop-filter: blur(3px);
      z-index: 999;
      opacity: 0;
      transition: opacity 0.3s ease;
    }
    .sidebar-overlay.active { display: block; opacity: 1; }

    /* ============ SCROLL TO TOP ============ */
    .scroll-top-btn {
      position: fixed;
      bottom: 24px; right: 24px;
      width: 48px; height: 48px;
      border-radius: 50%;
      background: var(--grad-btn);
      color: white;
      border: none;
      font-size: 1.2rem;
      cursor: pointer;
      box-shadow: 0 6px 20px rgba(76,175,80,0.4);
      z-index: 900;
      display: flex; align-items: center; justify-content: center;
      opacity: 0;
      visibility: hidden;
      transition: all 0.3s ease;
      padding: 0;
    }
    .scroll-top-btn.show { opacity: 1; visibility: visible; }
    .scroll-top-btn:hover { transform: translateY(-3px) scale(1.08); }

    /* ============ AUDIO CONTROLS ============ */
    #audio-controls {
      margin-top: 20px;
      display: none;
      align-items: center;
      gap: 10px;
      flex-wrap: wrap;
      justify-content: center;
    }
    #audio-controls button {
      background: rgba(255,255,255,0.2);
      color: white;
      border: 1px solid white;
      padding: 8px 16px;
      border-radius: 20px;
      cursor: pointer;
      margin: 0;
    }
    #audio-controls input[type="range"] { width: 150px; }

    /* ============ RESPONSIVE ============ */
    @media (max-width: 992px) {
      .sidebar { transform: translateX(-100%); }
      .sidebar.open { transform: translateX(0); }
      .content-area { margin-left: 0; }
      .menu-toggle-btn { display: flex; }
      .topbar { padding: 12px 18px; }
      main.container { padding: 28px 18px 20px; }
      .hero { padding: 40px 18px 36px; }
      .hero .hiasan { height: 200px; }
    }

    @media (max-width: 600px) {
      .topbar-title { font-size: 0.95rem; }
      .topbar-icon-btn { width: 38px; height: 38px; font-size: 1rem; }
      .menu-toggle-btn { width: 38px; height: 38px; }
      .card { padding: 18px; }
      .card h2 { font-size: 1.15rem; }
      .about-content { padding: 20px 18px; }
      .btn-about { top: auto; bottom: 18px; right: 18px; }
      .scroll-top-btn { bottom: 80px; }
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

    <div id="audio-controls" style="display: none;">
      <button id="mute-btn">🔇 Mute</button>
      <input type="range" id="volume-slider" min="0" max="100" value="80">
    </div>
  </div>

  <!-- ============ KONTEN UTAMA ============ -->
  <div class="main-content">
    <div class="app-layout">

      <!-- ============ SIDEBAR ============ -->
      <aside class="sidebar" id="sidebar">
        <div class="sidebar-brand">
          <div class="brand-logo">🌿</div>
          <div class="brand-text">
            <h3>LeafZuya</h3>
            <p>Have Fun Web</p>
          </div>
        </div>

        <nav class="sidebar-nav">
          <div class="nav-section-label">Menu</div>
          <a class="nav-item active" href="#home" data-nav>
            <span class="nav-icon">🏠</span> Home
          </a>
          <a class="nav-item" href="#tentang" data-nav>
            <span class="nav-icon">✨</span> Tentang
          </a>
          <a class="nav-item" href="#game" data-nav>
            <span class="nav-icon">🎮</span> Mini Games
          </a>
          <a class="nav-item" href="#karya" data-nav>
            <span class="nav-icon">📂</span> Karya
          </a>

          <div class="nav-section-label">Lainnya</div>
          <a class="nav-item" href="#ttt-card" data-nav>
            <span class="nav-icon">🎯</span> Tic-Tac-Toe
          </a>
          <a class="nav-item" href="#donasi" data-nav>
            <span class="nav-icon">🇵🇸</span> Donasi
          </a>
          <a class="nav-item" href="mailto:kingglafeon@gmail.com">
            <span class="nav-icon">📧</span> Kirim Saran
          </a>
          <a class="nav-item" href="https://trakteer.id/leafzuya%28daffa%29" target="_blank">
            <span class="nav-icon">🍵</span> Traktir
          </a>
          <button class="nav-item" id="aboutBtn2">
            <span class="nav-icon">ℹ️</span> Info Website
          </button>
        </nav>

        <div class="sidebar-footer">
          <button class="theme-toggle-btn" id="themeToggle">
            <span id="themeIcon">🌙</span>
            <span id="themeLabel">Dark Mode</span>
          </button>
        </div>
      </aside>

      <div class="sidebar-overlay" id="sidebarOverlay"></div>

      <!-- ============ CONTENT AREA ============ -->
      <div class="content-area">

        <!-- TOP BAR -->
        <div class="topbar">
          <button class="menu-toggle-btn" id="menuToggle" aria-label="Menu">☰</button>
          <div class="topbar-title">LeafZuya <span>Web</span> 🌿</div>
          <div class="topbar-actions">
            <button class="topbar-icon-btn" id="themeToggleTop" title="Toggle Dark Mode">🌙</button>
            <button class="topbar-icon-btn btn-about" id="aboutBtn" title="Tentang">ℹ️</button>
          </div>
        </div>

        <!-- HERO -->
        <header class="hero" id="home">
          <img src="Iwak.gif" alt="Foto Karya" class="hiasan">
          <h1>🌟 Welcome to My First Web 🌟</h1>
          <p>Dibuat oleh LeafZuya (Daffa) 😎🤭</p>
          <div class="emoji-decor emoji1">🍀</div>
          <div class="emoji-decor emoji2">✨</div>
          <div class="emoji-decor emoji3">💙</div>
        </header>

        <!-- JAM DIGITAL -->
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

        <!-- BUBBLES -->
        <div class="bubble green" style="left: 10%; width: 40px; height: 40px; animation-duration: 14s;"></div>
        <div class="bubble blue" style="left: 30%; width: 25px; height: 25px; animation-duration: 12s;"></div>
        <div class="bubble green" style="left: 50%; width: 50px; height: 50px; animation-duration: 16s;"></div>
        <div class="bubble blue" style="left: 70%; width: 30px; height: 30px; animation-duration: 11s;"></div>
        <div class="bubble green" style="left: 90%; width: 35px; height: 35px; animation-duration: 13s;"></div>

        <main class="container">
          <div class="cards-masonry">

            <!-- Card: Tentang -->
            <div class="card" id="tentang">
              <h2>✨ Tentang 🍀</h2>
              <p>Website ini dibuat cuma buat have fun aja, bukan serius. Jadi enjoyyy 😙</p>
              <p>Kirim kritik dan saran kalian ke <a href="mailto: kingglafeon@gmail.com">Gmail Ku [LeafZuya(Daffa)]....hehehe...🥳</a></p>

              <div style="text-align:center; margin:30px 0;">
                <a href="https://trakteer.id/leafzuya%28daffa%29" target="_blank">
                  <button style="background: linear-gradient(135deg, #ff4e50, #f9d423); border: none; padding: 15px 35px; border-radius: 40px; color: white; font-size: 1.2rem; font-weight: bold; cursor: pointer; box-shadow: 0 5px 15px rgba(0,0,0,0.2); transition: all 0.3s ease;">
                    🍵 Bagi yang mau Traktir......buat Beli Laptop ♥️🥳
                  </button>
                </a>

                <button onclick="playMusic('Jokowi.mp3')">Jangan Pencet Aku....☠️🗿</button>
                <audio id="audio1" src="Jokowi.mp3"></audio>

                <button onclick="playMusic('gok.mp3')">Jangan Pencet Aku....☠️🗿v2</button>
                <audio id="audio2" src="gok.mp3"></audio>

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
                </script>
                <b>JANGAN COBA-COBA SCREENSHOOT CODE QR DIBAWAH INI,LALU MEMINDAI NYA DI PEMINDAI QR CODE 🗿☠️💀</b>
                <img src="Idiot.jpg" alt="Gambar Karya" width="200" height="200" style="border-radius: 15px; margin-top: 12px;">
              </div>
            </div>

            <!-- Card: Quiz Kemerdekaan -->
            <div class="card" id="game" style="border: 3px solid #000; background: linear-gradient(135deg, #d90000, #ffffff, #ff0202, #e3b1b1); color: #000; box-shadow: 0 0 10px rgba(0,0,0,0.4);">
              <h2 style="text-align:center; color:#000; font-weight:bold;">🇮🇩QUIZ SPESIAL HARI KEMERDEKAAN (Limited Event)🔥</h2>

              <div style="text-align:center; margin-bottom:15px;">
                <div class="gold-frame" onclick="playFrameSound()">
                  <img src="Merdeka.png" alt="Support Palestine">
                </div>

                <audio id="frameSound" src="IDN.mp3"></audio>
                <script>
                  function playFrameSound() {
                    const audio = document.getElementById("frameSound");
                    audio.currentTime = 0;
                    audio.play();
                  }
                </script>
              </div>

              <div class="donate-btn-wrapper">
                <a href="Miami.html" target="_blank" class="donate-btn">
                  <img src="MerdekaT.png" alt="Donasi Palestina">
                </a>
              </div>

              <p style="text-align:center; background:#ff5c5c; padding:10px; border-radius:10px; color:#fff;">
                <b>"🇮🇩 'Bangsaku yang tercinta, janganlah kamu lupa pada sejarah perjuanganmu. Karena dari sanalah kita belajar untuk terus maju.'"</b><br>
                <b>~By:LeafZuya</b>
              </p>

              <p style="text-align:center; background:#ffffff; padding:10px; border-radius:10px; color:#000;">Gass Aja Mainin,bakal Di Tutup saat <b>25 Agustus 2026</b> Awokawokawok</p>
            </div>

            <!-- Card: Donasi Palestina -->
            <div class="card" id="donasi" style="border: 3px solid #000; background: linear-gradient(135deg, #1a1a1a, #ffffff, #009739, #ce1126); color: #000; box-shadow: 0 0 10px rgba(0,0,0,0.4);">
              <h2 style="text-align:center; color:#000; font-weight:bold;">🇵🇸 Donasi Untuk Palestina</h2>

              <div style="text-align:center; margin-bottom:15px;">
                <div class="gold-frame" onclick="playFrameSound2()">
                  <img src="Palestina.jpg" alt="Support Palestine">
                </div>
                <audio id="frameSound2" src="Free.mp3"></audio>
                <script>
                  function playFrameSound2() {
                    const audio = document.getElementById("frameSound2");
                    audio.currentTime = 0;
                    audio.play();
                  }
                </script>
              </div>

              <div class="donate-btn-wrapper">
                <a href="https://www.rumahzakat.org/donasi/palestina" target="_blank" class="donate-btn">
                  <img src="PalestinaT.jpg" alt="Donasi Palestina">
                </a>
              </div>

              <p style="text-align:center; background:#fff; padding:10px; border-radius:10px; color:#000;">
                Bantu saudara-saudara kita di Palestina yang sedang mengalami krisis kemanusiaan.
                Sepeser Bantuan kecil dari kalian dapat memberi dampak besar bagi mereka.
                🇵🇸💚 Terima kasih untuk kebaikan hati kalian.<br>
                <b>~By:LeafZuya</b>
              </p>

              <p style="text-align:center; background:#fff; padding:10px; border-radius:10px; color:#000;">Nanti Kalian Akan Diarahkan Ke <b>WEBSITE/SITUS RESMI DAN AMAN</b> untuk Menyumbangkan Amal Sumbangan...Jadi Uang-Nya Tidak Masuk Ke <b>REKENING PRIBADI-KU</b> Yahh!!...</p>
            </div>

            <!-- Card: Pelajaran -->
            <div class="card">
              <h2>📘 Pelajaran Favorit</h2>
              <p>Matematika & Informatika 💚💙 Karena Melatih Berpikir Kritis dalam menyelesaikan Sesuatu Masalah...!!!!! hehe...gak jelas ah...</p>
            </div>

            <!-- Card: Hobi -->
            <div class="card">
              <h2>🎮 Hobi 🎶</h2>
              <p>Main game, coding iseng-iseng, dan punya mimpi jadi Indie GameDev 🥳🤞</p>
            </div>

            <!-- Card: Video -->
            <div class="card">
              <h2>📺 Video Random</h2>
              <iframe width="220" height="220" src="https://www.youtube.com/embed/hyd8vfuQta0"
                title="YouTube video player" frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

              <iframe width="220" height="220" src="https://www.youtube.com/embed/nhUVc_9ki44"
                title="YouTube video player" frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>

            <!-- Card: Karya Danang -->
            <div class="card" id="karya">
              <h2>Penasaran Karya Danang...?, Klik Dibawah Ini ya...!😋</h2><br>
              <a href="https://leafzuya.github.io/Khusus_Danang/">Klik aku untuk melihat berbagai Karya Buatan Danang.....😆</a><br>
              <a>Jangan Lupa Follow Akun Media Sosialnya...!!</a><br>
              <a href="https://tiktok.com/@zainaki_and_hoshino">Media Sosial Danang </a>
            </div>

            <!-- TIC TAC TOE -->
            <div class="card" id="ttt-card">
              <h2>🎯 Tic-Tac-Toe — Player vs AI</h2>
              <p style="margin-bottom:12px;">Pilih sisi & tingkat kesulitan, lalu kalahkan AI kalau bisa 😎</p>

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
                   style="--cell:94px; margin:0 auto; width:calc(var(--cell)*3); display:grid; grid-template-columns:repeat(3,1fr); gap:10px;">
              </div>

              <div id="ttt-status" style="margin-top:14px; font-weight:600; color:#2e7d32;">Status: siap!</div>
              <div id="ttt-score" style="margin-top:6px; opacity:.9;">Skor — Kamu: <span id="s-you">0</span> | AI: <span id="s-ai">0</span> | Seri: <span id="s-draw">0</span></div>

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
                  boardEl.classList.remove('done');
                  setStatus("Giliran: " + glyph(turn));
                  maybeAiFirst();
                }

                function glyph(p){ return p==='X'?'❌ X':'⭕ O'; }

                function maybeAiFirst(){
                  if (turn === ai){ setTimeout(()=> aiMove(), 250); }
                }

                function setStatus(t){ statusEl.textContent = "Status: " + t; }

                function humanMove(i){
                  if (finished || turn!==human || board[i]) return;
                  pushHistory();
                  place(i, human);
                  afterMove();
                }

                function aiMove(){
                  if (finished || turn!==ai) return;
                  const diff = selDiff.value;
                  let move;
                  if (diff === 'easy') move = randomMove();
                  else if (diff === 'medium') move = bestMove({maxDepth:2, jitter:true});
                  else if (diff === 'hard') move = bestMove({maxDepth:6});
                  else move = bestMove({maxDepth:9});
                  pushHistory();
                  place(move, ai, true);
                  afterMove();
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

            <!-- Card: Tangkap Emoji -->
            <div class="card">
              <h2>Tangkap Emoji....!!😎🥳😵</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="Emoji.jpg" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/Web-Have-Fun-/">Klik aku untuk Mainkan...!!!,Kalo kalah, Berarti Noob😎☝️</a>
              <p>Cara mainnya tinggal di Klik ke kanan atau ke kiri aja,lalu tangkap semua dan kumpulkan point sebanyak-banyaknya.....!!!(Hanya disediakan 3 Nyawa/Kesempatan)</p>
            </div>

            <!-- Card: Sound Memory -->
            <div class="card">
              <h2>Sound Memory....!!🗣️🎤🎧</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="Simon.jpg" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/Sound-Memori-/">Klik aku untuk Mainkan sound memori...!!!,Kalo cepat kalah, Berarti jangan main ini lagi,main sana game Roblox 🤓☝️</a>
              <p>Cara mainnya tinggal ikuti irama yang muncul acak dan pencet tombol sesuai irama yang muncul pada tombol tersebut.....semakin lama akan semakin banyak irama yang akan di putar/mainkan..... Semangat....!!!🥳♥️🔥</p>
            </div>

            <!-- Card: Kalkulator -->
            <div class="card">
              <h2>Kalkulator LeafZuya 😆🌿➗➖➕</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="Kalkulator.jpg" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/Kalkulator-/">Klik aku untuk Menjalankan Kalkulator,versi Buatan ku sendiri.....</a>
              <p>Konon katanya,orang yang menggunakan Kalkulator Ini,bisa menambahkan IQ Manusia Maksimal sampai 105....🗿👍</p>
            </div>

            <!-- Card: LeafCy AI -->
            <div class="card">
              <h2>LeafCy AI😆🌿</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="leafcy.png" alt="Foto Karya" class="hiasan">
              <a href="https://leafcyai.my.id/" class="magic-btn">Kunjungi LeafCy AI☘️😆</a>
              <p>Jangan Lupa Klik Tombol Diatas yah....Itu adalah AI Buatan ku Sendiri (LeafZuya),tapi masih Tahap Pengembangan (Beta)...kalian juga bisa Tambahkan Obrolan dan Jawaban Obrolan Nya...[LeafCy AI X OpenRouter]😆🤞☘️🍃</p>
            </div>

            <!-- Card: Leaf-Wheel -->
            <div class="card">
              <h2>Leaf-Wheel🎡🌿</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="Wheel.jpg" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/Leaf_Wheel/" class="magic-btn">Kunjungi Leaf-Wheel☘️🎡</a>
              <p>Butuh Roda Penentu Keberuntungan???, Cobain Leaf-Wheel Yukkk!!!!🗿🙏☘️🎡</p>
            </div>

            <!-- Card: Cek Hewan -->
            <div class="card">
              <h2>Cek Hewan Dalam Jiwa Kalian!!🌿</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="Hewan.jpg" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/Cek-Hewan-/" class="magic-btn">Kunjungi Cek Hewan Dalam Jiwa ☘️✅🗿</a>
              <p>Apakah Kalian Sering Bertanya Dalam Hati"Sebenarnya, Apasih Hewan/Khodam Dalam Diri ku ini?"...Nahh,untuk itu, Kunjungi Minigame Diatas,untuk Memecahkan Rasa Penasaran Kamu...🗿🙏☕</p>
            </div>

            <!-- Card: LeafPy -->
            <div class="card">
              <h2>LeafPy!🐦🌿</h2>
              <p><b>Dibawah ini Hanya Gambar Ilustrasi saja!!</b></p>
              <img src="LeafPy.jpg" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/LeafPy/" class="magic-btn">Game Burung Santai, selamat Bermain  ☕🗿🍃🐦</a>
              <p>Kalian Suka Tantangan Skor Paling Banyak Dengan Orang lain Di Seluruh Dunia???,Nahhh...kalian Datang Di tempat yang Tepat,Di LeafPy,Kalian Bisa Mengumpulkan Skor sebanyak-banyaknya dengan cara melewati Rintangan Pipa Merah!!!, Minigame Ini juga Dilengkapi Leaderboard Online Mengandalkan Server Storage Browser....(Butuh Waktu 4 Minggu Woilah Baru Selesai 🗿🙏☕)</p>
            </div>

            <!-- Card: LeafFast -->
            <div class="card">
              <h2>Uji Kekuatan Kecepatan Jari!🌿</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="Fast.jpg" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/LeafFast/" class="magic-btn">Kunjungi LeafFast ☘️✅🗿</a>
              <p>Apakah Kalian Mempunyai Kekuatan Kecepatan Super???,Kalo iya,buktikan Dengan Memainkan Minigame ini🗿🙏☕</p>
            </div>

            <!-- Card: Leaf Flip -->
            <div class="card">
              <h2>Uji Ingatan Otak!🌿</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="Flip.png" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/Leaf_Flip/" class="magic-btn">Mainkan Supaya Punya IQ tinggi!☘️🗿</a>
              <p>Ingin Punya Ingatan Super???,Ingin Punya IQ Tingi???,Nahh...Mainkan Lah,Minigame Ini!🗿🙏☕</p>
            </div>

            <!-- Card: Sneaky -->
            <div class="card">
              <h2>Sneaky!🌿🗿</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="Sneak.jpg" alt="Foto Karya" class="hiasan">
              <a href="https://leafzuya.github.io/Sneaky/" class="magic-btn">Mainkan Sneaky! ☘️🗿</a>
              <p>Game Gabut Final Bos,Tema Nostalgia+Jadul,tapi Dengan Nuansa Dan Fitur Modern!🗿🙏☕</p>
            </div>

            <!-- Card: ReflexZ -->
            <div class="card">
              <h2>ReflexZ😆🌿</h2>
              <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
              <img src="ReflexZ.png" alt="Foto Karya" class="hiasan">
              <a href="ReflexZ.html" class="magic-btn">Kunjungi ReflexZ!😆</a>
              <p>Gas Aja Mainin,ga Usah Basa-Basi🤞🍃</p>
            </div>

          </div>
        </main>

        <!-- ABOUT PAGE -->
        <section id="aboutPage" class="about-page">
          <div class="about-content">
            <h2>🌿 LeafZuya Web Have Fun</h2>
            <p>
              Website ini dibuat sebagai hiburan Di Waktu Luang,Jangan Terlalu Fokus/Serius pada Website ini,Hidup kalian lebih berwarna,jika kalian melakukan Hal-Hal yang Bermanfaat untuk Orang lain dan Diri Sendiri...Ingat!,kita Ini Makhluk Yang Lemah!,Jangan Sombong kepada sang Pencipta!,Karena Dialah yang Berkuasa atas Dunia Ini,dan Jangan Lupa <b>BERBUAT BAIK</b> 💚.
            </p><br>

            <p>Website Ini Dipercayai Oleh 150+ Orang² Gabut dari Seluruh Dunia,dan Diawasi Oleh Organisasi Perkumpulan Orang² Gabut Se-Asia Tenggara(OPO2GAT)</p>

            <ul>
              <li>Dibuat Sejak:10 Agustus 2025
                <li><b>🧩 Versi:</b> v17.8.45— "Blood Leaves of Struggle🇮🇩🔥"</li>
                <li><b>💬 Dibuat oleh:</b> <span style="color:#09b;">LeafZuya(Daffa)</span></li>
            </ul>

            <p class="dev-note">
              ✨ Catatan Developer:<br>
              "Ubahlah Waktu Luang Kalian Yang Tidak Bermanfaat,Menjadi <b>SEDIKIT</b> lebih Bermanfaat"
            </p>
            <li><b>📅 Update terakhir:</b> 16 Agustus 2026</li>
            <h1> •Apa Yang Baru?</h1>
            <p>-Memperbaiki Bug</p>
            <p>-Mengubah Deskripsi dan Gambar Ilustrasi LeafCy AI</p>
            <p>-Update LeafCy AI,Jadi Punya Logikanya Sendiri!!😆</p>
            <p>-Update LeafCy Jadi Punya Akselerasi buat Mengetik "Zuya Ganteng 😎 " Sebanyak 1000x,Untuk Me-Redeem Pengurangan Waktu Selama 30 Menit🗿🙏</p>

            <button id="backBtn" class="btn-back">⬅️ Kembali</button>
          </div>
        </section>

        <!-- FOOTER -->
        <footer>
          © 2025 Fun Web by LeafZuya. Jangan Copyright...!! dan Jangan Lupa
          <b>BERNAFAS</b> 🤭🗣️🔥<br>
          <span class="footer-emoji">🍀</span>
          <span class="footer-emoji">💚</span>
          <span class="footer-emoji">💙</span>
        </footer>
      </div>
    </div>
  </div>

  <!-- SCROLL TO TOP -->
  <button class="scroll-top-btn" id="scrollTopBtn" title="Kembali ke atas">⬆️</button>

  <!-- ============ SCRIPT: SIDEBAR, THEME, NAV ============ -->
  <script>
  (function() {
    const sidebar = document.getElementById('sidebar');
    const overlay = document.getElementById('sidebarOverlay');
    const menuToggle = document.getElementById('menuToggle');

    function openSidebar() {
      sidebar.classList.add('open');
      overlay.classList.add('active');
    }
    function closeSidebar() {
      sidebar.classList.remove('open');
      overlay.classList.remove('active');
    }

    if (menuToggle) menuToggle.addEventListener('click', openSidebar);
    if (overlay) overlay.addEventListener('click', closeSidebar);

    // Tutup sidebar saat nav item diklik (mobile)
    document.querySelectorAll('[data-nav]').forEach(el => {
      el.addEventListener('click', () => {
        if (window.innerWidth <= 992) closeSidebar();
      });
    });

    // Active nav highlight saat scroll
    const navItems = document.querySelectorAll('[data-nav]');
    const sections = [];
    navItems.forEach(n => {
      const id = n.getAttribute('href');
      if (id && id.startsWith('#')) {
        const sec = document.querySelector(id);
        if (sec) sections.push({ id: id, el: sec, nav: n });
      }
    });

    function updateActiveNav() {
      let current = sections[0];
      const scrollPos = window.scrollY + 140;
      sections.forEach(s => {
        if (s.el.offsetTop <= scrollPos) current = s;
      });
      navItems.forEach(n => n.classList.remove('active'));
      if (current) current.nav.classList.add('active');
    }
    window.addEventListener('scroll', updateActiveNav);

    // ============ THEME TOGGLE ============
    const body = document.body;
    const themeToggle = document.getElementById('themeToggle');
    const themeToggleTop = document.getElementById('themeToggleTop');
    const themeIcon = document.getElementById('themeIcon');
    const themeLabel = document.getElementById('themeLabel');

    function applyTheme(isDark) {
      if (isDark) {
        body.classList.add('dark-mode');
        if (themeIcon) themeIcon.textContent = '☀️';
        if (themeLabel) themeLabel.textContent = 'Light Mode';
        if (themeToggleTop) themeToggleTop.textContent = '☀️';
      } else {
        body.classList.remove('dark-mode');
        if (themeIcon) themeIcon.textContent = '🌙';
        if (themeLabel) themeLabel.textContent = 'Dark Mode';
        if (themeToggleTop) themeToggleTop.textContent = '🌙';
      }
    }

    // Load saved theme
    try {
      const saved = localStorage.getItem('leafzuya-theme');
      if (saved === 'dark') applyTheme(true);
      else applyTheme(false);
    } catch (e) { applyTheme(false); }

    function toggleTheme() {
      const isDark = !body.classList.contains('dark-mode');
      applyTheme(isDark);
      try { localStorage.setItem('leafzuya-theme', isDark ? 'dark' : 'light'); } catch(e) {}
    }

    if (themeToggle) themeToggle.addEventListener('click', toggleTheme);
    if (themeToggleTop) themeToggleTop.addEventListener('click', toggleTheme);

    // ============ ABOUT PAGE ============
    const aboutPage = document.getElementById('aboutPage');
    const aboutBtn = document.getElementById('aboutBtn');
    const aboutBtn2 = document.getElementById('aboutBtn2');
    const backBtn = document.getElementById('backBtn');

    function showAbout() { aboutPage.classList.add('show'); }
    function hideAbout() { aboutPage.classList.remove('show'); }

    if (aboutBtn) aboutBtn.addEventListener('click', showAbout);
    if (aboutBtn2) aboutBtn2.addEventListener('click', () => { showAbout(); if (window.innerWidth <= 992) closeSidebar(); });
    if (backBtn) backBtn.addEventListener('click', hideAbout);

    // ============ SCROLL TO TOP ============
    const scrollTopBtn = document.getElementById('scrollTopBtn');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 400) scrollTopBtn.classList.add('show');
      else scrollTopBtn.classList.remove('show');
    });
    scrollTopBtn.addEventListener('click', () => {
      window.scrollTo({ top: 0, behavior: 'smooth' });
    });
  })();
  </script>

  <!-- ============ SCRIPT LOADING SCREEN (ASLI) ============ -->
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
          console.log("Auto-play dicegah, tunggu interaksi user:", error);
          loadingText.textContent = "Klik tombol 'Start' untuk memutar musik...";
          startButton.addEventListener('click', function playOnInteraction() {
            loadingAudio.play().then(() => {
              console.log("Audio diputar setelah interaksi");
              startButton.removeEventListener('click', playOnInteraction);
            });
          }, { once: true });
        });
      }
    }

    if (volumeSlider && loadingAudio) {
      volumeSlider.addEventListener('input', function() {
        loadingAudio.volume = this.value / 100;
        if (this.value == 0) muteBtn.innerHTML = '🔇 Mute';
        else muteBtn.innerHTML = '🔊 Unmute';
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

  <!-- ============ SCRIPT JAM DIGITAL (ASLI) ============ -->
  <script>
  function updateJamDigital() {
    const now = new Date();
    let jam24 = now.getHours();
    const menit = now.getMinutes().toString().padStart(2, '0');
    const detik = now.getSeconds().toString().padStart(2, '0');
    const ampm = jam24 >= 12 ? 'PM' : 'AM';
    const jamFormatted = jam24.toString().padStart(2, '0');

    const jamMenitElem = document.getElementById('jamMenitUtama');
    if (jamMenitElem) {
      jamMenitElem.innerHTML = `${jamFormatted}<span class="titik-jam">:</span>${menit}`;
    }
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
</body>
</html>
