# Project-gabut-Daffa-LeafZuya-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Login - LeafZuya Website</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #00c6ff, #0072ff);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .login-box {
      background: white;
      padding: 25px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(0,0,0,0.2);
      width: 300px;
      text-align: center;
    }
    .login-box h2 {
      margin-bottom: 20px;
      color: #333;
    }
    .login-box input {
      width: 90%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 8px;
    }
    .login-box button {
      width: 95%;
      padding: 10px;
      background: #0072ff;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      margin-top: 10px;
    }
    .login-box button:hover {
      background: #0055cc;
    }
    .message {
      margin-top: 10px;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="login-box">
    <h2>🔑 Login</h2>
    <input type="text" id="username" placeholder="Username"><br>
    <input type="password" id="password" placeholder="Password"><br>
    <button onclick="login()">Login</button>
    <p class="message" id="message"></p>
  </div>

  <script>
    function login() {
      const user = document.getElementById("username").value;
      const pass = document.getElementById("password").value;
      const msg = document.getElementById("message");

      // Username & Password sementara
      const correctUser = "LeafZuya";
      const correctPass = "12345";

      if (user === correctUser && pass === correctPass) {
        msg.style.color = "green";
        msg.textContent = "Login berhasil! 🚀";

        // Redirect ke halaman utama setelah login
        setTimeout(() => {
          window.location.href = "index.html";
        }, 1000);
      } else {
        msg.style.color = "red";
        msg.textContent = "Username atau Password salah ❌";
      }
    }
  </script>
</body>
</html>
