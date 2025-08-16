<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>RajWeb - Home</title>
  <style>
    :root{
      --page-bg: #FFEB3B; /* yellow page */
      --boys: #1976D2;    /* blue */
      --girls: #2E7D32;   /* green */
      --card-radius: 14px;
      --shadow: 0 6px 18px rgba(0,0,0,0.12);
      --font: "Segoe UI", Roboto, Arial, sans-serif;
    }

    html,body{
      height:100%;
      margin:0;
      font-family:var(--font);
      background:var(--page-bg);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .container{
      min-height:100%;
      display:flex;
      flex-direction:column;
      align-items:center;
      justify-content:center;
      gap:28px;
      padding:24px;
      box-sizing:border-box;
    }

    h1{
      margin:0;
      font-size:24px;
      text-align:center;
      color:#222;
      font-weight:600;
    }

    .boxes{
      display:flex;
      gap:20px;
      flex-wrap:wrap;
      justify-content:center;
    }

    .box{
      width:200px;
      height:140px;
      border-radius:var(--card-radius);
      box-shadow:var(--shadow);
      display:flex;
      align-items:center;
      justify-content:center;
      color:white;
      font-size:20px;
      font-weight:700;
      cursor:pointer;
      user-select:none;
      text-decoration:none;
      transition:transform .14s ease, box-shadow .14s ease;
    }

    .box:active{ transform:scale(.98); }
    .box:hover{ transform:translateY(-6px); box-shadow:0 14px 30px rgba(0,0,0,0.18); }

    .boys { background:var(--boys); }
    .girls { background:var(--girls); }

    /* small note under boxes */
    .note{
      font-size:14px;
      color:#222;
      opacity:.9;
      margin-top:4px;
      text-align:center;
    }

    /* responsive */
    @media (max-width:420px){
      .box{ width:160px; height:120px; font-size:18px; }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>pgp College students III - BSC CS</h1>

    <div class="boxes">
      <!-- Link to details page -->
      <a class="box boys" href="details.html?group=boys" title="Boys - click to see details">Boys (Click here)</a>

      <a class="box girls" href="details.html?group=girls" title="Girls - click to see details">Girls (Click here)</a>
    </div>

    <div class="note">
      Webpage colour: Yellow • Boys box: Blue • Girls box: Green
    </div>
  </div>
</body>
</html>
