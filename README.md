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
    (function () {
      cons
