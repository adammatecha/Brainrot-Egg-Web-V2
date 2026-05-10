# Brainrot Egg Website 😄

Vytvoř nový soubor `index.html` a vlož tam CELÝ tento kód:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Brainrot Egg</title>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Poppins',sans-serif;
    }

    body{
      background:linear-gradient(180deg,#060616,#0e1030,#18144d);
      color:white;
      overflow-x:hidden;
    }

    .bg-glow{
      position:fixed;
      width:600px;
      height:600px;
      background:#7c3aed;
      filter:blur(180px);
      opacity:0.25;
      top:-200px;
      left:-150px;
      z-index:-1;
      animation:moveGlow 10s infinite alternate;
    }

    @keyframes moveGlow{
      from{
        transform:translateY(0px);
      }
      to{
        transform:translateY(80px);
      }
    }

    nav{
      display:flex;
      justify-content:space-between;
      align-items:center;
      padding:25px 8%;
      backdrop-filter:blur(10px);
      position:sticky;
      top:0;
      background:rgba(0,0,0,0.25);
      border-bottom:1px solid rgba(255,255,255,0.1);
      z-index:999;
    }

    .logo{
      font-size:32px;
      font-weight:700;
      color:#a855f7;
      text-shadow:0 0 20px #a855f7;
    }

    .nav-links{
      display:flex;
      gap:30px;
    }

    .nav-links a{
      text-decoration:none;
      color:white;
      transition:0.3s;
    }

    .nav-links a:hover{
      color:#a855f7;
    }

    .hero{
      min-height:90vh;
      display:flex;
      justify-content:center;
      align-items:center;
      flex-direction:column;
      text-align:center;
      padding:40px;
    }

    .hero h1{
      font-size:90px;
      line-height:1;
      max-width:1000px;
      text-shadow:0 0 30px rgba(168,85,247,0.6);
    }

    .hero p{
      margin-top:25px;
      color:#cfcfe7;
      font-size:22px;
      max-width:700px;
    }

    .hero button{
      margin-top:40px;
      background:linear-gradient(90deg,#7c3aed,#c026d3);
      border:none;
      color:white;
      padding:18px 40px;
      border-radius:18px;
      font-size:22px;
      cursor:pointer;
      transition:0.3s;
      box-shadow:0 0 30px rgba(168,85,247,0.5);
    }

    .hero button:hover{
      transform:scale(1.06);
    }

    .section-title{
      text-align:center;
      font-size:52px;
      margin-top:50px;
      margin-bottom:40px;
    }

    .cards{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:25px;
      padding:0 8% 80px;
    }

    .card{
      background:rgba(255,255,255,0.06);
      border:1px solid rgba(255,255,255,0.08);
      border-radius:28px;
      padding:35px;
      backdrop-filter:blur(15px);
      transition:0.3s;
      box-shadow:0 0 30px rgba(0,0,0,0.25);
    }

    .card:hover{
      transform:translateY(-8px);
      border-color:#a855f7;
    }

    .card h2{
      font-size:32px;
      margin-bottom:10px;
    }

    .rarity{
      display:inline-block;
      margin-top:10px;
      padding:8px 18px;
      border-radius:999px;
      font-size:15px;
      font-weight:600;
    }

    .common{
      background:#3f3f46;
    }

    .rare{
      background:#2563eb;
    }

    .epic{
      background:#9333ea;
    }

    .legendary{
      background:#f59e0b;
      color:black;
    }

    .status-box{
      margin:0 auto 90px;
      width:85%;
      max-width:900px;
      background:rgba(255,255,255,0.06);
      border-radius:30px;
      padding:40px;
      border:1px solid rgba(255,255,255,0.1);
      text-align:center;
      box-shadow:0 0 40px rgba(168,85,247,0.2);
    }

    .status{
      display:inline-block;
      margin-top:18px;
      background:#f59e0b;
      color:black;
      padding:12px 24px;
      border-radius:999px;
      font-weight:700;
      animation:pulse 2s infinite;
    }

    @keyframes pulse{
      0%{
        transform:scale(1);
      }
      50%{
        transform:scale(1.05);
      }
      100%{
        transform:scale(1);
      }
    }

    .footer{
      text-align:center;
      padding:35px;
      color:#9ca3af;
      border-top:1px solid rgba(255,255,255,0.08);
    }

    @media(max-width:800px){
      .hero h1{
        font-size:52px;
      }

      .nav-links{
        display:none;
      }
    }
  </style>
</head>
<body>

<div class="bg-glow"></div>

<nav>
  <div class="logo">BRAINROT EGG</div>

  <div class="nav-links">
    <a href="#">Home</a>
    <a href="#">Rarities</a>
    <a href="#">Status</a>
    <a href="#">Leaks</a>
  </div>
</nav>

<section class="hero">
  <h1>THE MOST BRAINROT EGG EXPERIENCE</h1>

  <p>
    Discover insane eggs, crazy rarities and secret updates.
    Something BIG is coming soon 😈
  </p>

  <button>PLAY SOON</button>
</section>

<h1 class="section-title">RARITIES</h1>

<div class="cards">

  <div class="card">
    <h2>Capy Egg</h2>
    <p>Funny beginner egg with chaotic energy.</p>
    <div class="rarity common">COMMON</div>
  </div>

  <div class="card">
    <h2>Brainrot Cube Egg</h2>
    <p>Mysterious glowing cube with cursed power.</p>
    <div class="rarity rare">RARE</div>
  </div>

  <div class="card">
    <h2>Galaxy Egg</h2>
    <p>Contains unknown cosmic brainrot.</p>
    <div class="rarity epic">EPIC</div>
  </div>

  <div class="card">
    <h2>VOID EGG</h2>
    <p>The rarest egg ever discovered.</p>
    <div class="rarity legendary">LEGENDARY</div>
  </div>

</div>

<div class="status-box">
  <h1>GAME STATUS</h1>

  <p style="margin-top:20px;font-size:22px;color:#d1d5db;">
    The game is currently being reworked.
    Massive update and new systems are in development.
  </p>

  <div class="status">⚠ UNDER REWORK ⚠</div>
</div>

<div class="footer">
  © 2026 Brainrot Egg • Made by Adam 😄
</div>

</body>
</html>
```

Potom:

1. Klikni dole na `Commit changes`
2. Jdi do `Settings`
3. `Pages`
4. Source → `Deploy from branch`
5. Vyber `main`
6. Save

A za pár minut bude web online 🚀
