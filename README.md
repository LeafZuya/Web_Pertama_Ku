# Web-Have-Fun
<html lang="id">
<head>
  <meta name="google-site-verification" content="df6EtL6mKtOPWlg4bi57__R4cjbLIAuNwZisuD42fHo" />
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
<b>JANGAN COBA-COBA UNDUH CODE QR DIBAWAH INI,LALU MEMINDAI NYA DI PEMINDAI QR CODE 🗿☠️💀</b>
<!-- Gambar bisa dilihat & diunduh -->
<a href="Idiot.jpg" download>
  <img src="Idiot.jpg" alt="Gambar Karya" width="200" height="200>
</a>
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
  <img src="Emoji.jpg" width="220" height="220">
      <a href="https://leafzuya.github.io/Web-Have-Fun-/">Klik aku untuk Mainkan...!!!,Kalo kalah, Berarti Noob😎☝️</a>
  <p>Cara mainnya tinggal di Klik ke kanan atau ke kiri aja,lalu tangkap semua dan kumpulkan point sebanyak-banyaknya.....!!!(Hanya disediakan 3 Nyawa/Kesempatan)</p>
    </div>

    <div class="card">
      <h2>Sound Memory....!!🗣️🎤🎧</h2>
      <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
      <img src="Simon.jpg" width="220" height="220">
      <a href="https://leafzuya.github.io/Sound-Memori-/">Klik aku untuk Mainkan sound memori...!!!,Kalo cepat kalah, Berarti jangan main ini lagi,main sana game Roblox 🤓☝️</a>
  <p>Cara mainnya tinggal ikuti irama yang muncul acak dan pencet tombol sesuai irama yang muncul pada tombol tersebut.....semakin lama akan semakin banyak irama yang akan di putar/mainkan..... Semangat....!!!🥳♥️🔥</p>
    </div>
    <div class="card">
      <h2>Kalkulator LeafZuya 😆🌿➗➖➕</h2>
      <p>dibawah ini,hanya Ilustrasi gambar...jadi,percuma Di-Klik² berapa kali pun </p>
      <img src="Kalkulator.jpg" width="220" height="220">
      <a href="https://leafzuya.github.io/Kalkulator-/">Klik aku untuk Menjalankan Kalkulator,versi Buatan ku sendiri.....</a>
  <p>Konon katanya,orang yang menggunakan Kalkulator Ini,bisa menambahkan IQ Manusia Maksimal sampai 105....🗿👍</p>
    </div>


  <footer>
    © 2025 Fun Web by LeafZuya. Jangan Copyright...!! dan Jangan Lupa <b>BERNAFAS</b> 🤭🗣️🔥<br>
    <span class="footer-emoji">🍀</span>
    <span class="footer-emoji">💚</span>
    <span class="footer-emoji">💙</span>
  </footer>

