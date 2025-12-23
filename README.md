# 100-Girlfriends-Cup-
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>100 Girlfriends Cup</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #0a1a3a; /* navy blue */
      color: gold;
    }
    header {
      text-align: center;
      padding: 20px;
    }
    header img {
      max-height: 120px;
      display: block;
      margin: 0 auto 10px;
    }
    h1 {
      font-size: 40px;
      margin: 0;
    }
    nav {
      text-align: center;
      margin: 20px;
    }
    nav button {
      background: gold;
      color: #0a1a3a;
      border: none;
      padding: 10px 20px;
      margin: 0 5px;
      cursor: pointer;
      font-weight: bold;
    }
    .container {
      padding: 20px;
    }
    .group, .match, .bracket {
      border: 1px solid gold;
      margin-bottom: 15px;
      padding: 10px;
    }
    .match button {
      margin: 5px;
      background: transparent;
      color: gold;
      border: 1px solid gold;
      cursor: pointer;
    }
    footer {
      text-align: center;
      padding: 15px;
      border-top: 1px solid gold;
    }
    .hidden { display: none; }
    input, select {
      padding: 5px;
      margin: 5px 0;
    }
  </style>
</head>
<body>
  <header>
    <img id="logo" src="" alt="Tournament Logo" />
    <h1>100 Girlfriends Cup</h1>
  </header>  <nav>
    <button onclick="showPage('groups')">Group Stages</button>
    <button onclick="showPage('knockout')">Knockout Stage</button>
    <button onclick="showPage('admin')">Admin</button>
  </nav>  <div class="container">
    <div id="groups">
      <h2>Group Stages</h2>
      <div id="groupContainer"></div>
    </div><div id="knockout" class="hidden">
  <h2>Knockout Bracket</h2>
  <div class="bracket" id="qf">Quarter Finals</div>
  <div class="bracket" id="sf">Semi Finals</div>
  <div class="bracket" id="final">Final</div>
</div>

<div id="admin" class="hidden">
  <h2>Admin Panel</h2>
  <input type="password" id="adminPass" placeholder="Admin Password" />
  <button onclick="
