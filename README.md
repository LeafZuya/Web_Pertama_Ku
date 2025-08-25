# Project-Random-ApaSajaLah
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
      <h2>📸 Galeri SpesialZzZz</h2>
      <iframe width="220" height="220" src="https://www.youtube.com/embed/tucpVglVsi4"
      title="YouTube video player" frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

      <div class="card">
  <h2>🎮 Minigame: Tic Tac Toe</h2>
  <div id="tic-tac-toe"></div>
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
<!-- 🧠♟️ CARD: CHESS vs AI -->
<div class="card" id="chess-card">
  <h2>♟️ Catur vs AI</h2>
  <div style="display:grid;grid-template-columns:1fr;gap:14px;justify-items:center;">
    <div id="board" style="width: 360px;"></div>

    <div style="display:flex;gap:10px;flex-wrap:wrap;justify-content:center;">
      <button id="btn-new">🔁 New Game</button>
      <button id="btn-undo">↩️ Undo</button>
      <button id="btn-flip">🔃 Flip Board</button>
    </div>

    <div style="display:flex;gap:10px;align-items:center;flex-wrap:wrap;justify-content:center;">
      <label for="sel-skill"><b>Level AI:</b></label>
      <select id="sel-skill">
        <option value="1">1 (kebun baru)</option>
        <option value="5">5</option>
        <option value="10" selected>10 (menantang)</option>
        <option value="15">15</option>
        <option value="20">20 (dewa)</option>
      </select>

      <label for="sel-movetime"><b>Waktu Pikir AI:</b></label>
      <select id="sel-movetime">
        <option value="200">0.2s</option>
        <option value="500" selected>0.5s</option>
        <option value="1000">1s</option>
        <option value="2000">2s</option>
        <option value="5000">5s</option>
      </select>
    </div>

    <div id="status" style="font-weight:600;color:#2e7d32;">Status: Siap</div>
    <div id="lastMove" style="font-size:0.95rem;color:#444;"></div>
  </div>
</div>
<!-- 🎨 chessboard.js CSS -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.css" integrity="sha512-aQ1M5E1sMoa0q2Q5gYy8bDg6GSJ3a5jC8U14U+W2j0uQ0cC6V2Wc7cOxx4fKf3wB85e7mZP1b0L8M7k1m0Fq6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />

<!-- 🧩 chessboard.js + chess.js (aturan catur) -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/chessboard.js/1.0.0/chessboard-1.0.0.min.js" integrity="sha512-8W8h0R3b5z7M5nqH1Hc4v8v7e0hGkXv3nDg9sQn9Z1r2bJwzQm0hJQk5uVw8Nw9oB5h0v8mJr0o7cVv6qG4s7Q==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.10.3/chess.min.js" integrity="sha512-wJrY0aHq2nXEUyq1N2o7i4c3e1Oq3n1XYcG8G9L3F0vK3m8l9G8i4tQ6m8mQyDgL8eC8m0v2Jk5bqjJv1a2H7A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>

<!-- 🧠 Stockfish (AI). Jika gagal, kita pakai fallback AI sederhana -->
<script src="https://cdn.jsdelivr.net/npm/stockfish@16/stockfish.js"></script>

<script>
(() => {
  // ======== STATE & SETUP ========
  const statusEl   = document.getElementById('status');
  const lastMoveEl = document.getElementById('lastMove');
  const skillSel   = document.getElementById('sel-skill');
  const timeSel    = document.getElementById('sel-movetime');

  let game   = new Chess();
  let board  = null;
  let engine = null;      // Stockfish instance
  let usingEngine = false;
  let boardFlipped = false;
  let engineReady = false;
  let pendingBestMove = null;

  // ======== INIT BOARD ========
  function onDragStart (source, piece, position, orientation) {
    if (game.game_over()) return false;
    // Hanya boleh gerak pion putih kalau orientasi white; kita biarkan player = side to move
    if ((game.turn() === 'w' && piece.search(/^b/) !== -1) ||
        (game.turn() === 'b' && piece.search(/^w/) !== -1)) return false;
  }

  function onDrop (source, target) {
    // Cek legalitas langkah
    const move = game.move({ from: source, to: target, promotion: 'q' });
    if (move === null) return 'snapback';

    updateStatus(move);
    window.requestAnimationFrame(() => {
      board.position(game.fen());
      if (!game.game_over()) {
        // Giliran AI
        setTimeout(aiMove, 50);
      }
    });
  }

  function onSnapEnd () {
    board.position(game.fen());
  }

  function updateStatus (lastMove) {
    let status = '';

    const moveColor = (game.turn() === 'w') ? 'Putih' : 'Hitam';

    if (game.in_checkmate()) {
      status = 'Skakmat! ' + (moveColor === 'Putih' ? 'Hitam' : 'Putih') + ' menang.';
    } else if (game.in_draw()) {
      status = 'Seri (draw).';
    } else {
      status = 'Giliran: ' + moveColor + (game.in_check() ? ' — SKAK!' : '');
    }

    statusEl.textContent = 'Status: ' + status;

    if (lastMove) {
      lastMoveEl.textContent = 'Langkah terakhir: ' +
        (lastMove.color === 'w' ? 'Putih ' : 'Hitam ') +
        lastMove.from + ' → ' + lastMove.to + (lastMove.promotion ? ' (promosi ' + lastMove.promotion + ')' : '');
    }
  }

  board = Chessboard('board', {
    draggable: true,
    position: 'start',
    moveSpeed: 'fast',
    snapSpeed: 'fast',
    snapbackSpeed: 400,
    onDragStart,
    onDrop,
    onSnapEnd,
  });

  // ======== STOCKFISH ENGINE INIT ========
  try {
    if (typeof STOCKFISH === 'function') {
      engine = STOCKFISH(); // main-thread engine object (tanpa worker)
      usingEngine = true;
      setupEngine();
    }
  } catch (e) {
    usingEngine = false;
  }

  function setupEngine () {
    // Komunikasi UCI
    engine.onmessage = function (line) {
      const text = ('' + line).trim();
      // console.log('SF:', text);

      if (text === 'uciok') {
        engineReady = true;
        // set skill
        engine.postMessage('setoption name Skill Level value ' + (+skillSel.value));
        statusEl.textContent = 'Status: Engine siap. Giliran Putih.';
      }

      if (text.startsWith('bestmove')) {
        const parts = text.split(' ');
        const best = parts[1];
        pendingBestMove = best;
      }
    };

    // init UCI
    engine.postMessage('uci');
  }

  function engineGo (fen, movetimeMs) {
    pendingBestMove = null;
    engine.postMessage('ucinewgame');
    engine.postMessage('position fen ' + fen);
    engine.postMessage('go movetime ' + movetimeMs);
  }

  function uciToMoveObj (uci) {
    // e.g., "e2e4", "e7e8q"
    if (!uci || uci.length < 4) return null;
    const from = uci.substring(0,2);
    const to   = uci.substring(2,4);
    const prom = uci.length > 4 ? uci[4] : undefined;
    return { from, to, promotion: prom };
  }

  // ======== FALLBACK AI (kalau Stockfish gagal) ========
  const PIECE_VALUE = { p: 100, n: 320, b: 330, r: 500, q: 900, k: 20000 };
  function evaluateBoard (chess) {
    let total = 0;
    const board = chess.board();
    for (let r = 0; r < 8; r++) {
      for (let c = 0; c < 8; c++) {
        const p = board[r][c];
        if (!p) continue;
        const val = PIECE_VALUE[p.type] || 0;
        total += (p.color === 'w') ? val : -val;
      }
    }
    return total;
  }

  function pickMoveFallback (chess, depth = 2) {
    function minimax (d, alpha, beta, maximizing) {
      if (d === 0 || chess.game_over()) return evaluateBoard(chess);

      const moves = chess.moves();
      if (maximizing) {
        let maxEval = -Infinity;
        for (const m of moves) {
          chess.move(m);
          const evalv = minimax(d-1, alpha, beta, false);
          chess.undo();
          if (evalv > maxEval) maxEval = evalv;
          if (evalv > alpha) alpha = evalv;
          if (beta <= alpha) break;
        }
        return maxEval;
      } else {
        let minEval = Infinity;
        for (const m of moves) {
          chess.move(m);
          const evalv = minimax(d-1, alpha, beta, true);
          chess.undo();
          if (evalv < minEval) minEval = evalv;
          if (evalv < beta) beta = evalv;
          if (beta <= alpha) break;
        }
        return minEval;
      }
    }

    const moves = chess.moves({ verbose: true });
    let best = null;
    let bestScore = -Infinity;

    for (const m of moves) {
      chess.move(m);
      const score = minimax(depth-1, -Infinity, Infinity, false);
      chess.undo();
      if (score > bestScore) { bestScore = score; best = m; }
    }
    return best ? { from: best.from, to: best.to, promotion: best.promotion } : null;
  }

  // ======== AI MOVE ========
  function aiMove () {
    if (game.game_over()) return;

    // Coba pakai Stockfish dulu
    if (usingEngine && engine && engineReady) {
      engineGo(game.fen(), +timeSel.value);
      const waitStart = performance.now();

      const tick = () => {
        if (pendingBestMove) {
          const mv = uciToMoveObj(pendingBestMove);
          const res = game.move(mv);
          if (res) {
            updateStatus(res);
            board.position(game.fen());
          }
          pendingBestMove = null;
          return;
        }
        // safety timeout 8s
        if (performance.now() - waitStart > 8000) {
          // fallback
          usingEngine = false;
          fallbackAndMove();
          return;
        }
        requestAnimationFrame(tick);
      };
      requestAnimationFrame(tick);
      return;
    }

    // Kalau engine ga ada / gagal, fallback
    fallbackAndMove();
  }

  function fallbackAndMove () {
    const skill = +skillSel.value;
    // Depth fallback kasar: 2..4
    const depth = Math.max(2, Math.min(4, Math.round(skill/5)+1));
    const mv = pickMoveFallback(game, depth);
    if (mv) {
      const res = game.move(mv);
      if (res) {
        updateStatus(res);
        board.position(game.fen());
      }
    }
  }

  // ======== CONTROLS ========
  document.getElementById('btn-new').addEventListener('click', () => {
    game.reset();
    board.start();
    updateStatus();
  });

  document.getElementById('btn-undo').addEventListener('click', () => {
    // Undo dua langkah (player & AI) biar kembali ke giliran player
    game.undo();
    game.undo();
    board.position(game.fen());
    updateStatus();
  });

  document.getElementById('btn-flip').addEventListener('click', () => {
    boardFlipped = !boardFlipped;
    board.orientation(boardFlipped ? 'black' : 'white');
  });

  skillSel.addEventListener('change', () => {
    if (engine && usingEngine) {
      engine.postMessage('setoption name Skill Level value ' + (+skillSel.value));
    }
  });

  updateStatus();
})();
</script>
  </main>

  <footer>
    © 2025 Fun Web by LeafZuya. Jangan Copyright...!! dan Jangan Lupa <b>BERNAFAS</b> 🤭🗣️🔥<br>
    <span class="footer-emoji">🍀</span>
    <span class="footer-emoji">💚</span>
    <span class="footer-emoji">💙</span>
  </footer>
</body>
</html>
