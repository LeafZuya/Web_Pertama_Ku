# Web-Have-Fun
<html lang="id">
<head>
  <meta name="google-site-verification" content="df6EtL6mKtOPWlg4bi57__R4cjbLIAuNwZisuD42fHo" />
  <title>Fun Web by LeafZuya (Daffa)</title>
  
  <link rel="icon" href="Favicon.ico" type="image/x-icon">
<link rel="icon" href="favicon.png" type="image/png">

<!-- 🌿 Untuk Android dan Chrome -->
<link rel="apple-touch-icon" sizes="180x180" href="https://leafzuya.github.io/Web_Pertama_Ku/favicon.png">
<link rel="manifest" href="https://leafzuya.github.io/Web_Pertama_Ku/manifest.json">
<!-- 🌐 SEO Meta Tags -->
<meta name="title" content="LeafZuya Web — Have Fun">
<meta name="description" content="LeafZuya Website khusus untuk orang-orang yang sedang mencari kesenangan di waktu luang 🌿💙">
<meta name="keywords" content="LeafCy, LeafZuya, AI Chat, Virtual Friend, Artificial Intelligence, Blue Archive Inspired, Web AI Indonesia, Web Have Fun, Karya Anak Gabut">
<meta name="author" content="LeafZuya (Daffa)">

<!-- 📱 Open Graph (Facebook, Discord, Google Rich Preview) -->
<meta property="og:title" content="LeafZuya Web — Have Fun">
<meta property="og:description" content="Website ini dibuat hanya karena kegabutan LeafZuya — dan sekadar hobi di waktu luang 😆">
<meta property="og:image" content="https://leafzuya.github.io/Web_Pertama_Ku/Favicon.png">
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

    /* Container Card (grid default) */
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

    /* 🔥 Tambahan Solusi Kedua: Masonry Layout */
    .container {
      column-count: 3;       /* jumlah kolom, bisa diubah */
      column-gap: 25px;      /* jarak antar kolom */
    }

    .card {
      display: inline-block; /* wajib untuk masonry */
      width: 100%;
      margin: 0 0 25px;
    }

    /* Responsif masonry */
    @media (max-width: 768px) {
      .container { column-count: 2; }
    }
    @media (max-width: 480px) {
      .container { column-count: 1; }
    }
  .hiasan {
    width: 400px;
    height: 250px;
    border: 8px solid transparent;
    border-radius: 30px; /* sudut jadi tumpul */
    background: linear-gradient(135deg, #4caf50, #2196f3); /* Hijau → Biru */
    padding: 5px; /* jarak antara border & gambar */
    box-shadow: 0 8px 20px rgba(0,0,0,0.3); /* bayangan */
  }
  </style>
</head>
<body>
  <header>
    <img src="Iwak.gif" alt="Foto Karya" class="hiasan">
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
    
       Kirim kritik dan saran kalian ke <a href="mailto: kingglafeon@gmail.com">Gmail Ku [LeafZuya(Daffa)]....hehehe...🥳</a>

         <div style="text-align:center; margin:30px;">
  <a href="https://trakteer.id/leafzuya%28daffa%29" target="_blank">
    <button style="
      background: linear-gradient(135deg, #ff4e50, #f9d423);
      border: none;
      padding: 15px 35px;
      border-radius: 40px;
      color: white;
      font-size: 1.2rem;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
      transition: all 0.3s ease;">
      🍵 Bagi yang mau Traktir......buat Beli Laptop ♥️🥳
    </button>
  </a>

  <!-- Tombol -->
<button onclick="playMusic()">Jangan Pencet Aku....☠️🗿</button>

<!-- Audio -->
<audio id="myAudio" src="Jokowi.mp3"></audio>
<!-- ganti "music/bgmusic.mp3" sesuai lokasi file MP3 kamu -->

<script>
  function playMusic() {
    const audio = document.getElementById("myAudio");
    audio.play();
  }
</script>
<b>JANGAN COBA-COBA SCREENSHOOT CODE QR DIBAWAH INI,LALU MEMINDAI NYA DI PEMINDAI QR CODE 🗿☠️💀</b>

<img src="Idiot.jpg" alt="Gambar Karya" width="200" height="200">

</div>
     
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
      <h2>Penasaran Karya Danang...?, Klik Dibawah Ini ya...!😋</h2><br>
      
   <a href="https://leafzuya.github.io/Khusus_Danang/">Klik aku untuk melihat berbagai Karya Buatan Danang.....😆</a><br>

   <a>Jangan Lupa Follow Akun Media Sosialnya...!!</a><br>
   
  <a href="https://tiktok.com/@zainaki_and_hoshino">Media Sosial Danang </a>
    </div>

     <!-- === TIC TAC TOE: Player vs AI (paste this inside <main class="container">) === -->
<div class="card" id="ttt-card">
  <h2>🎯 Tic-Tac-Toe — Player vs AI</h2>
  <p style="margin-bottom:12px;">Pilih sisi & tingkat kesulitan, lalu kalahkan AI kalau bisa 😎</p>

  <!-- Controls -->
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

  <!-- Board -->
  <div id="ttt-board"
       style="--cell:94px; margin:0 auto; width:calc(var(--cell)*3); display:grid; grid-template-columns:repeat(3,1fr); gap:10px;">
    <!-- cells generated by JS -->
  </div>

  <!-- Status + Score -->
  <div id="ttt-status" style="margin-top:14px; font-weight:600; color:#2e7d32;">Status: siap!</div>
  <div id="ttt-score" style="margin-top:6px; opacity:.9;">Skor — Kamu: <span id="s-you">0</span> | AI: <span id="s-ai">0</span> | Seri: <span id="s-draw">0</span></div>

  <!-- Styles scoped -->
  <style>
    #ttt-board .ttt-cell{
      height:var(--cell); aspect-ratio:1/1; display:flex; align-items:center; justify-content:center;
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

    /* Buttons tweak to match your theme */
    #ttt-card button{
      background: linear-gradient(135deg, #4caf50, #2196f3);
      border: none; padding: 10px 16px; border-radius: 24px; color: #fff;
      font-weight:700; cursor:pointer; box-shadow: 0 8px 15px rgba(0,0,0,.2); transition: transform .15s ease, box-shadow .2s ease;
    }
    #ttt-card button:hover{ transform: translateY(-2px); box-shadow:0 12px 22px rgba(0,0,0,.25);}
    #ttt-card select{ background:#fff; }
    /* Responsive board */
    @media (max-width:420px){
      #ttt-board{ --cell:86px; gap:8px; width:calc(var(--cell)*3); }
    }
    @media (max-width:360px){
      #ttt-board{ --cell:78px; gap:8px; width:calc(var(--cell)*3); }
    }
  </style>

  <!-- Logic -->
  <script>
  (function(){
    const boardEl = document.getElementById('ttt-board');
    const statusEl = document.getElementById('ttt-status');
    const sYou = document.getElementById('s-you'), sAi = document.getElementById('s-ai'), sDraw = document.getElementById('s-draw');
    const selSide = document.getElementById('ttt-side');
    const selDiff = document.getElementById('ttt-difficulty');
    const btnNew = document.getElementById('ttt-new'), btnUndo = document.getElementById('ttt-undo'), btnHint = document.getElementById('ttt-hint');

    // Game state
    let board, human, ai, turn, finished, history, scores = {you:0, ai:0, draw:0};
    const lines = [[0,1,2],[3,4,5],[6,7,8],[0,3,6],[1,4,7],[2,5,8],[0,4,8],[2,4,6]];
    const TT = new Map(); // transposition table (hash -> {score, best})

    // Build cells
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
      if (turn === ai){
        setTimeout(()=> aiMove(), 250);
      }
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
      else move = bestMove({maxDepth:9}); // impossible
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
      if (res){
        endGame(res);
        return;
      }
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
      // disable clicks
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

    // Undo
    function pushHistory(){ history.push({board:[...board], turn, finished}); }
    function undo(){
      if (!history.length) return;
      const prev = history.pop();
      board = prev.board;
      turn = prev.turn;
      finished = prev.finished;
      cells.forEach((c,i)=> {
        c.textContent = board[i]||'';
        c.classList.remove('win','disabled','played');
        if (board[i]) c.classList.add('played');
      });
      setStatus("Undo. Giliran: " + glyph(turn));
    }

    // Hint
    function hint(){
      if (finished || board.every(v=>v)) return;
      const move = (turn===ai) ? bestMove({maxDepth: selDiff.value==='impossible'?9:6})
                               : (selDiff.value==='easy'?randomMove():bestMove({maxDepth:4, jitter:true}));
      if (move==null) return;
      cells[move].style.boxShadow = "0 0 0 3px rgba(33,150,243,.7) inset, 0 12px 22px rgba(0,0,0,.2)";
      setTimeout(()=> cells[move].style.boxShadow='', 650);
    }

    // AI — Minimax + Alpha-Beta with TT
    function bestMove({maxDepth=9, jitter=false}={}){
      const me = ai, opp = human;
      const key0 = hash(board, turn);
      // Move ordering: center, corners, edges
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
        // Prefer faster wins / slower losses
        const val = (w.win===me) ? (10 - depth) : (depth - 10);
        return val;
      }
      if (depth>=9) return 0; // full 3x3 depth safe-guard

      const key = hash(b, toMove);
      const tt = TT.get(key);
      if (tt && tt.depth >= depth) return tt.score;

      // move ordering
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

    // Events
    btnNew.addEventListener('click', reset);
    btnUndo.addEventListener('click', undo);
    btnHint.addEventListener('click', hint);
    selSide.addEventListener('change', reset);
    selDiff.addEventListener('change', reset);

    // init
    reset();
  })();
  </script>
</div>
<!-- === /TIC TAC TOE === -->

<div class="card">
      <h2>Tangkap Emoji....!!😎🥳😵</h2>
  <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
  <img src="Emoji.jpg" alt="Foto Karya" class="hiasan">
      <a href="https://leafzuya.github.io/Web-Have-Fun-/">Klik aku untuk Mainkan...!!!,Kalo kalah, Berarti Noob😎☝️</a>
  <p>Cara mainnya tinggal di Klik ke kanan atau ke kiri aja,lalu tangkap semua dan kumpulkan point sebanyak-banyaknya.....!!!(Hanya disediakan 3 Nyawa/Kesempatan)</p>
    </div>

    <div class="card">
      <h2>Sound Memory....!!🗣️🎤🎧</h2>
      <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
      
   <img src="Simon.jpg" alt="Foto Karya" class="hiasan">
     
  <a href="https://leafzuya.github.io/Sound-Memori-/">Klik aku untuk Mainkan sound memori...!!!,Kalo cepat kalah, Berarti jangan main ini lagi,main sana game Roblox 🤓☝️</a>
  <p>Cara mainnya tinggal ikuti irama yang muncul acak dan pencet tombol sesuai irama yang muncul pada tombol tersebut.....semakin lama akan semakin banyak irama yang akan di putar/mainkan..... Semangat....!!!🥳♥️🔥</p>
    </div>
    <div class="card">
      <h2>Kalkulator LeafZuya 😆🌿➗➖➕</h2>
      <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
      <img src="Kalkulator.jpg" alt="Foto Karya" class="hiasan">
      <a href="https://leafzuya.github.io/Kalkulator-/">Klik aku untuk Menjalankan Kalkulator,versi Buatan ku sendiri.....</a>
  <p>Konon katanya,orang yang menggunakan Kalkulator Ini,bisa menambahkan IQ Manusia Maksimal sampai 105....🗿👍</p>
    </div>

    <div class="card">
      <h2>LeafCy AI😆🌿</h2>
      <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
      
  <img src="LeafCy.jpg" alt="Foto Karya" class="hiasan">
     
      <!-- 🌿 Tombol Unik Hijau-Biru -->
<a href="https://leafzuya.github.io/Chat-With-LeafCy/" class="magic-btn">Kunjungi LeafCy AI☘️😆</a>

<style>
.magic-btn {
  display: inline-block;
  padding: 14px 26px;
  font-size: 17px;
  font-weight: 700;
  color: white;
  text-decoration: none;
  border-radius: 18px; /* Sudut tumpul */
  background: linear-gradient(135deg, #00e69a, #1ea7ff);
  box-shadow: 0 6px 20px rgba(0, 150, 136, 0.4);
  transition: all 0.25s ease;
  position: relative;
  overflow: hidden;
}

/* Efek kilau lembut */
.magic-btn::after {
  content: "";
  position: absolute;
  top: 0;
  left: -75%;
  width: 50%;
  height: 100%;
  background: rgba(255, 255, 255, 0.3);
  transform: skewX(-25deg);
  transition: all 0.6s ease;
}

/* Efek hover */
.magic-btn:hover {
  transform: scale(1.07);
  box-shadow: 0 10px 28px rgba(0, 150, 255, 0.5);
}

.magic-btn:hover::after {
  left: 125%;
}
</style>
  <p>Jangan Lupa Klik Tombol Diatas yah....Itu adalah AI Buatan ku Sendiri (LeafZuya),tapi masih Tahap Pengembangan (Beta)...kalian juga bisa Tambahkan Obrolan dan Jawaban Obrolan Nya...Bareng LeafCy 😆🤞☘️🍃</p>
    </div>

    <div class="card">
      <h2>Leaf-Wheel🎡🌿</h2>
      <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
      
  <img src="Wheel.jpg" alt="Foto Karya" class="hiasan">
     
      <!-- 🌿 Tombol Unik Hijau-Biru -->
<a href="https://leafzuya.github.io/Leaf_Wheel/" class="magic-btn">Kunjungi Leaf-Wheel☘️🎡</a>

<style>
.magic-btn {
  display: inline-block;
  padding: 14px 26px;
  font-size: 17px;
  font-weight: 700;
  color: white;
  text-decoration: none;
  border-radius: 18px; /* Sudut tumpul */
  background: linear-gradient(135deg, #00e69a, #1ea7ff);
  box-shadow: 0 6px 20px rgba(0, 150, 136, 0.4);
  transition: all 0.25s ease;
  position: relative;
  overflow: hidden;
}

/* Efek kilau lembut */
.magic-btn::after {
  content: "";
  position: absolute;
  top: 0;
  left: -75%;
  width: 50%;
  height: 100%;
  background: rgba(255, 255, 255, 0.3);
  transform: skewX(-25deg);
  transition: all 0.6s ease;
}

/* Efek hover */
.magic-btn:hover {
  transform: scale(1.07);
  box-shadow: 0 10px 28px rgba(0, 150, 255, 0.5);
}

.magic-btn:hover::after {
  left: 125%;
}
</style>
  <p>Butuh Roda Penentu Keberuntungan???, Cobain Leaf-Wheel Yukkk!!!!🗿🙏☘️🎡</p>
    </div>

    <div class="card">
      <h2>Cek Hewan Dalam Jiwa Kalian!!🌿</h2>
      <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
      
  <img src="Hewan.jpg" alt="Foto Karya" class="hiasan">
     
      <!-- 🌿 Tombol Unik Hijau-Biru -->
<a href="https://leafzuya.github.io/Cek-Hewan-/" class="magic-btn">Kunjungi Cek Hewan Dalam Jiwa ☘️✅🗿</a>

<style>
.magic-btn {
  display: inline-block;
  padding: 14px 26px;
  font-size: 17px;
  font-weight: 700;
  color: white;
  text-decoration: none;
  border-radius: 18px; /* Sudut tumpul */
  background: linear-gradient(135deg, #00e69a, #1ea7ff);
  box-shadow: 0 6px 20px rgba(0, 150, 136, 0.4);
  transition: all 0.25s ease;
  position: relative;
  overflow: hidden;
}

/* Efek kilau lembut */
.magic-btn::after {
  content: "";
  position: absolute;
  top: 0;
  left: -75%;
  width: 50%;
  height: 100%;
  background: rgba(255, 255, 255, 0.3);
  transform: skewX(-25deg);
  transition: all 0.6s ease;
}

/* Efek hover */
.magic-btn:hover {
  transform: scale(1.07);
  box-shadow: 0 10px 28px rgba(0, 150, 255, 0.5);
}

.magic-btn:hover::after {
  left: 125%;
}
</style>
  <p>Apakah Kalian Sering Bertanya Dalam Hati"Sebenarnya, Apasih Hewan/Khodam Dalam Diri ku ini?"...Nahh,untuk itu, Kunjungi Minigame Diatas,untuk Memecahkan Rasa Penasaran Kamu...🗿🙏☕</p>
    </div>

    <div class="card">
      <h2>LeafPy!🐦🌿</h2>
      <p><b>SEDANG DALAM PERBAIKAN!!!</b></p>
      
  <img src="Server.jpg" alt="Foto Karya" class="hiasan">
     
      <!-- 🌿 Tombol Unik Hijau-Biru -->
<a href="https://leafzuya.github.io/LeafPy/23" class="magic-btn">Sedang Dalam Perbaikan ☕🗿🍃🐦</a>

<style>
.magic-btn {
  display: inline-block;
  padding: 14px 26px;
  font-size: 17px;
  font-weight: 700;
  color: white;
  text-decoration: none;
  border-radius: 18px; /* Sudut tumpul */
  background: linear-gradient(135deg, #00e69a, #1ea7ff);
  box-shadow: 0 6px 20px rgba(0, 150, 136, 0.4);
  transition: all 0.25s ease;
  position: relative;
  overflow: hidden;
}

/* Efek kilau lembut */
.magic-btn::after {
  content: "";
  position: absolute;
  top: 0;
  left: -75%;
  width: 50%;
  height: 100%;
  background: rgba(255, 255, 255, 0.3);
  transform: skewX(-25deg);
  transition: all 0.6s ease;
}

/* Efek hover */
.magic-btn:hover {
  transform: scale(1.07);
  box-shadow: 0 10px 28px rgba(0, 150, 255, 0.5);
}

.magic-btn:hover::after {
  left: 125%;
}
</style>
  <p>Kalian Suka Tantangan Skor Paling Banyak Dengan Orang lain Di Seluruh Dunia???,Nahhh...kalian Datang Di tempat yang Tepat,Di LeafPy,Kalian Bisa Mengumpulkan Skor sebanyak-banyaknya dengan cara melewati Rintangan Pipa Merah!!!, Minigame Ini juga Dilengkapi Leaderboard Online Mengandalkan Lokal Storage Browser....(Butuh Waktu 5 Hari Woilah Baru Selesai 🗿🙏☕)</p>
    </div>
    
    <!-- Tombol menuju halaman Tentang -->
<button id="aboutBtn" class="btn-about">ℹ️ Tentang(Opsional,tapi Disarankan 🗿☕)</button>

<!-- Halaman Tentang (disembunyikan awalnya) -->
<section id="aboutPage" class="about-page">
  <div class="about-content">
    <h2>🌿 LeafZuya Web Have Fun</h2>
    <p>
      Website ini dibuat sebagai hiburan Di Waktu Luang,Jangan Terlalu Fokus/Serius pada Website ini,Hidup kalian lebih berwarna,jika kalian melakukan Hal-Hal yang Bermanfaat untuk Orang lain dan Diri Sendiri...Ingat!,kita Ini Makhluk Yang Lemah!,Jangan Sombong kepada sang Pencipta!,Karena Dialah yang Berkuasa atas Dunia Ini,dan Jangan Lupa <b>BERBUAT BAIK</b> 💚.
    </p>

    <ul>
      
      <li><b>🧩 Versi:</b> v1.3 — "Daun Mekar"</li>
      <li><b>💬 Dibuat oleh:</b> <span style="color:#09b;">LeafZuya(Daffa)</span></li>
    </ul>

    <p class="dev-note">
      ✨ Catatan Developer:<br>
      "Ubahlah Waktu Luang Kalian Yang Tidak Bermanfaat,Menjadi <b>SEDIKIT</b> lebih Bermanfaat"
    </p>
    <li><b>📅 Update terakhir:</b> 22 Oktober 2025</li>
      <h1> •Apa Yang Baru?</h1>
    <p>-Perbaikan Bug</p>
    <p>-Update Minigame <b>TANGKAP EMOJI</b></p>
    <p>-Update Minigame <b>KALKULATOR LEAFZUYA</b></p>
    <p>-Perbaikan Bug Pada <b>LEAFCY AI</b></p>
    <p>-Penambahan Minigame <b>CEK HEWAN DALAM JIWA</b></p>
   <p>Penambahan Minigame <b>LEAFPY </b></p>
    
    

    <button id="backBtn" class="btn-back">⬅️ Kembali</button>
  </div>
</section>

<style>
/* tombol tentang */
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

/* halaman Tentang */
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
}
.about-page.show {
  display: flex;
}

.about-content {
  background: rgba(255,255,255,0.9);
  border-radius: 20px;
  box-shadow: 0 8px 50px rgba(0,0,0,0.2), 0 0 60px rgba(255,240,150,0.4);
  padding: 26px 30px;
  max-width: 600px;
  width: 90%;
}

.about-content h2 {
  color: #046;
  margin-bottom: 12px;
  text-shadow: 0 2px 10px rgba(255,255,150,0.4);
}

.about-content p {
  font-size: 15px;
  line-height: 1.6;
}

.about-content ul {
  text-align: left;
  list-style: none;
  padding: 0;
  margin: 15px 0;
}
.about-content li {
  margin: 6px 0;
  font-size: 14.5px;
}

.dev-note {
  font-style: italic;
  font-size: 13.5px;
  margin-top: 14px;
  color: #155;
}

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
</style>

<script>
// Tombol "Tentang"
const aboutBtn = document.getElementById('aboutBtn');
const aboutPage = document.getElementById('aboutPage');
const backBtn = document.getElementById('backBtn');

// buka halaman tentang
aboutBtn.addEventListener('click', ()=>{
  aboutPage.classList.add('show');
});

// kembali ke halaman utama
backBtn.addEventListener('click', ()=>{
  aboutPage.classList.remove('show');
});
</script>

  <footer>
  © 2025 Fun Web by LeafZuya. Jangan Copyright...!! dan Jangan Lupa 
  <b>BERNAFAS</b> 🤭🗣️🔥<br>
  <span class="footer-emoji">🍀</span>
  <span class="footer-emoji">💚</span>
  <span class="footer-emoji">💙</span>
  <br>
</footer>

