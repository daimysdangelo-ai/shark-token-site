<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SharkToken - Le Roi des Memecoins</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Orbitron', sans-serif;
      background: linear-gradient(to bottom, #004080, #00c2cb);
      color: white;
      padding: 20px;
      overflow-x: hidden;
    }
    h1, h2 {
      text-align: center;
      color: #00ffff;
      text-shadow: 1px 1px 2px #000;
    }
    .section {
      background: rgba(0, 0, 0, 0.3);
      padding: 20px;
      margin: 20px auto;
      border-radius: 20px;
      max-width: 800px;
      box-shadow: 0 0 15px rgba(0, 255, 255, 0.5);
    }
    ul {
      list-style-type: "🦈 ";
      padding-left: 20px;
    }
    a {
      color: #00ffff;
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
    .button {
      display: inline-block;
      padding: 12px 20px;
      margin: 10px auto;
      background-color: #00c2cb;
      color: #000;
      font-weight: bold;
      border-radius: 10px;
      text-align: center;
    }
    .wallet {
      background-color: rgba(255, 255, 255, 0.1);
      padding: 10px;
      border-radius: 10px;
      font-family: monospace;
    }
    #countdown {
      display: block;
      text-align: center;
      font-size: 1.5em;
      margin-bottom: 10px;
      color: #00ffff;
      font-weight: bold;
      letter-spacing: 2px;
    }
    .logo-container {
      display: flex;
      justify-content: center;
      margin-bottom: 24px;
    }
    .logo-container img {
      max-width: 320px;
      width: 100%;
      height: auto;
      border-radius: 24px;
      box-shadow: 0 0 30px rgba(0,255,255,0.3);
      background: #0099a5;
      z-index: 10;
      position: relative;
    }

    /* Styles for animated sharks */
    .shark-anim {
      position: fixed;
      pointer-events: none;
      z-index: 1;
      will-change: transform, opacity;
      opacity: 0.85;
      transition: filter 0.2s;
      filter: drop-shadow(0 2px 10px #00c2cb88);
      animation: sway 2s infinite alternate ease-in-out;
    }

    @keyframes sway {
      0% { transform: translateY(0) rotate(-4deg);}
      100% { transform: translateY(8px) rotate(4deg);}
    }
    /* For content layers above sharks */
    .content-on-top {
      position: relative;
      z-index: 2;
    }
  </style>
</head>
<body>
  <!-- Animated Sharks -->
  <div id="shark-anim-canvas"></div>

  <div class="content-on-top">
    <div class="logo-container">
      <img src="shark-token.png" alt="SharkToken Logo" />
    </div>

    <h1>🦈 SharkToken</h1>
    <h2>Lancement prévu le 24 août 2025 🌊</h2>

    <div class="section">
      <div id="countdown">Chargement du compte à rebours...</div>
      <a href="#" class="button">🔗 Connecter Phantom Wallet</a>
    </div>

    <div class="section">
      <h2>📘 Whitepaper</h2>
      <p>
        SharkToken est un <strong>memecoin Solana</strong> minable, décentralisé, évolutif, brûlable, communautaire,
        conçu pour dominer les océans du Web3.
      </p>
      <ul>
        <li>Minage simulé</li>
        <li>Burn 0.5% par transaction</li>
        <li>Fusion possible en NFT</li>
        <li>DAO communautaire (décembre 2025)</li>
        <li>Utilité : acheter d'autres memecoins avec SHARK</li>
      </ul>
    </div>

    <div class="section">
      <h2>🗘️ Roadmap</h2>
      <ul>
        <li>24 août 2025 – Lancement officiel (minage + airdrop)</li>
        <li>Sept – Dashboard de minage</li>
        <li>Oct – Concours mèmes</li>
        <li>Nov – Utilisation SHARK pour memecoins</li>
        <li>Déc – DAO communautaire</li>
        <li>Janv – Fusion en NFT évolutifs</li>
        <li>Fév – Listing Raydium/Jupiter</li>
        <li>Mars – Marketplace NFT</li>
        <li>Avril – Bridge inter-blockchain</li>
        <li>Mai – Jeux Web3, staking, events</li>
      </ul>
    </div>

    <div class="section">
      <h2>📱 Réseaux</h2>
      <p>
        🔗 <a href="https://t.me/SharkTokenofficial" target="_blank">Rejoins-nous sur Telegram</a><br>
        🐦 <a href="https://x.com/TheSharkTokens?t=addC28E2ooVDo6tXaz3eig&s=09" target="_blank">Suis-nous sur X (Twitter)</a>
      </p>
    </div>

    <div class="section">
      <h2>💳 Wallet Fondateur</h2>
      <div class="wallet">3iPkLMmCFkwqABw7AiVUrjYpsYdcYak8Vn82Fn2abHGp</div>
    </div>
  </div>

  <script>
    // Countdown logic
    function updateCountdown() {
      // Date cible : 24 août 2025 à 12:00:00 UTC
      const target = new Date(Date.UTC(2025, 7, 24, 12, 0, 0));
      const now = new Date();
      const diff = target - now;
      const countdown = document.getElementById('countdown');
      if (diff <= 0) {
        countdown.textContent = "🚀 SharkToken est lancé !";
        return;
      }
      const days = Math.floor(diff / (1000 * 60 * 60 * 24));
      const hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
      const minutes = Math.floor((diff / (1000 * 60)) % 60);
      const seconds = Math.floor((diff / 1000) % 60);
      countdown.textContent = `⏳ ${days}j ${hours}h ${minutes}m ${seconds}s avant le lancement`;
    }
    setInterval(updateCountdown, 1000);
    updateCountdown();

    // Animated sharks logic
    // Use shark-token.png for the little sharks!
    function random(min, max) {
      return Math.random() * (max - min) + min;
    }

    function spawnSharks(count) {
      const canvas = document.getElementById('shark-anim-canvas');
      for(let i = 0; i < count; i++) {
        const img = document.createElement('img');
        img.className = 'shark-anim';
        img.src = "shark-token.png";
        // Randomize size and initial position
        const size = random(30, 70); // px
        img.style.width = size + "px";
        img.style.height = "auto";
        img.style.left = random(-10, 100) + "vw";
        img.style.top = random(-10, 100) + "vh";
        img.style.opacity = random(0.5, 0.9);

        // Animate sharks: random direction, speed, amplitude
        const duration = random(18, 48); // seconds for a loop
        const way = Math.random() > 0.5 ? 1 : -1;
        const delay = random(0, 24);
        const swimAnim = img.animate([
          { transform: `translate(0,0) scaleX(${way})`, filter: 'brightness(1)' },
          { transform: `translate(${way * random(400,800)}px,${random(-60,60)}px) scaleX(${way})`, filter: 'brightness(1.15)' }
        ], {
          duration: duration * 1000,
          delay: delay * 1000,
          iterations: Infinity,
          direction: 'alternate',
          easing: 'ease-in-out'
        });
        // Sway animation is handled by CSS keyframes

        canvas.appendChild(img);
      }
    }
    // Responsive: more sharks on desktop, fewer on mobile
    function sharkCount() {
      if(window.innerWidth < 600) return 35;
      if(window.innerWidth < 1024) return 60;
      return 100;
    }
    spawnSharks(sharkCount());

    // Optionally, respawn on resize (for responsiveness)
    window.addEventListener('resize', () => {
      const canvas = document.getElementById('shark-anim-canvas');
      canvas.innerHTML = '';
      spawnSharks(sharkCount());
    });
  </script>
</body>
</html>
