# heirloomproto
Heirloom Login
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Hamilton & Associates – Login</title>
  <style>
    body{font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,Arial;margin:0;background:#f6f7fb}
    .wrap{max-width:420px;margin:10vh auto;padding:32px;background:#fff;border-radius:16px;box-shadow:0 8px 24px rgba(0,0,0,.08)}
    h1{margin:0 0 8px}
    label{display:block;font-size:14px;margin:16px 0 6px;color:#334}
    input{width:100%;padding:12px 14px;border:1px solid #ccd2e0;border-radius:10px;font-size:14px}
    button{margin-top:18px;width:100%;padding:12px 14px;border:0;border-radius:10px;background:#1f6feb;color:#fff;font-weight:600;cursor:pointer}
    .error{margin-top:12px;color:#b00020;font-size:13px;display:none}
    .hint{margin-top:8px;font-size:12px;color:#667}
  </style>
</head>
<body>
  <div class="wrap">
    <h1>Sign in</h1>
    <p class="hint">Demo creds: <code>demo@hamilton.com</code> / <code>probate123</code></p>
    <label for="email">Email</label>
    <input id="email" type="email" autocomplete="username" placeholder="you@hamilton.com" />
    <label for="password">Password</label>
    <input id="password" type="password" autocomplete="current-password" placeholder="••••••••" />
    <button id="login">Log in</button>
    <div id="err" class="error">Incorrect email or password.</div>
  </div>
  <script>
    const OK_USER = "demo@hamilton.com";
    const OK_PASS = "probate123";
    const email = document.getElementById("email");
    const pass = document.getElementById("password");
    const err  = document.getElementById("err");
    document.getElementById("login").addEventListener("click", () => {
      const good = email.value.trim().toLowerCase() === OK_USER && pass.value === OK_PASS;
      if (good) {
        // For demo, redirect to your “dashboard” mock (another HTML page or Figma link)
        window.location.href = "dashboard.html";
      } else {
        err.style.display = "block";
      }
    });
  </script>
</body>
</html>
