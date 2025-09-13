<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Hamilton & Associates – Login</title>
  <style>
    body{font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial;margin:0;background:#f6f7fb}
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

    <!-- Use a FORM so Enter key works; prevent default submit in JS -->
    <form id="login-form" novalidate>
      <label for="email">Email</label>
      <input id="email" type="email" autocomplete="username" placeholder="you@hamilton.com" required />

      <label for="password">Password</label>
      <input id="password" type="password" autocomplete="current-password" placeholder="••••••••" required />

      <button type="submit" id="login">Log in</button>
      <div id="err" class="error">Incorrect email or password.</div>
    </form>
  </div>

  <script>
    (function () <!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Probate Dashboard (Demo)</title>
  <style>
    body{font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial;margin:0;background:#f6f7fb}
    .shell{display:flex;min-height:100vh}
    .nav{width:240px;background:#121826;color:#e9eef7;padding:24px}
    .nav h2{margin-top:0;font-size:18px}
    .nav a{display:block;color:#e9eef7;text-decoration:none;margin:10px 0}
    .main{flex:1;padding:32px}
    .card{background:#fff;border-radius:16px;box-shadow:0 8px 24px rgba(0,0,0,.08);padding:20px;margin-bottom:16px}
    .muted{color:#667}
  </style>
</head>
<body>
  <div class="shell">
    <aside class="nav">
      <h2>Hamilton & Assoc.</h2>
      <a href="#">Dashboard</a>
      <a href="#">Matters</a>
      <a href="#">Documents</a>
      <a href="#">Calendar</a>
      <a href="#">Beneficiaries</a>
    </aside>
    <main class="main">
      <h1>Welcome to the Probate Dashboard</h1>
      <div class="card">
        <strong>Active Matters</strong>
        <p class="muted">Estate of Jane Smith (VIC) — Drafting Affidavit<br>
        Estate of Robert Brown (NSW) — Awaiting Grant</p>
      </div>
      <div class="card">
        <strong>Next Deadlines</strong>
        <p class="muted">Affidavit due 20 Sept • Filing due 25 Sept</p>
      </div>
    </main>
  </div>
</body>
</html>

      cons
