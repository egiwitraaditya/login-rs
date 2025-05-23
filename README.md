# login-rs
Aplikasi login tiket rs
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <title>Login Aplikasi</title>
  <style>
    body {
      font-family: Arial;
      background: #f0f0f0;
      display: flex;
      height: 100vh;
      justify-content: center;
      align-items: center;
    }
    .login-box {
      background: white;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
      width: 300px;
    }
    .login-box h2 {
      text-align: center;
      margin-bottom: 20px;
    }
    .login-box input {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    .login-box button {
      width: 100%;
      padding: 10px;
      background: #3498db;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .login-box button:hover {
      background: #2980b9;
    }
  </style>
</head>
<body>
  <div class="login-box">
    <h2>Login</h2>
    <input type="text" id="username" placeholder="Username" />
    <input type="password" id="password" placeholder="Password" />
    <button onclick="login()">Masuk</button>
  </div>

  <script>
    function login() {
      const user = document.getElementById('username').value;
      const pass = document.getElementById('password').value;

      // Data login disimpan langsung di kode
      if (user === 'admin' && pass === '1234') {
        alert("Login berhasil!");
        // Di sini kamu bisa redirect ke halaman lain
        // window.location.href = "halaman-utama.html";
      } else {
        alert("Username atau password salah.");
      }
    }
  </script>
</body>
</html>
