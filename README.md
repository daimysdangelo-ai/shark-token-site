<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>THE SHARK TOKEN - Memecoin Solana</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Orbitron&display=swap');
  body {
    margin: 0; padding: 0;
    font-family: 'Orbitron', sans-serif;
    background: linear-gradient(to bottom, #001f3f, #004e92);
    color: #00ffff;
    overflow-x: hidden;
  }
  header {
    position: relative;
    padding: 30px 20px 10px 20px;
    background: rgba(0, 20, 70, 0.8);
    box-shadow: 0 0 20px #00ffff;
    text-align: center;
    z-index: 1000;
  }
  header h1 {
    margin: 0;
    font-size: 2.8em;
    text-shadow: 0 0 10px #00ffff;
  }
  header p {
    font-size: 1.2em;
    margin: 5px 0 0 0;
    color: #b3f0ff;
    font-weight: 600;
  }

  /* Animations de requins */
  .shark {
    position: absolute;
    width: 60px;
    animation: swim 15s linear infinite;
    opacity: 0.8;
    filter: drop-shadow(0 0 5px cyan);
  }
  .shark:nth-child(1) {
    top: 10%;
    left: -80px;
    animation-duration: 25s;
  }
  .shark:nth-child(2) {
    top: 40%;
    left: -100px;
    animation-duration: 20s;
  }
  .shark:nth-child(3) {
    top: 75%;
    left: -60px;
    animation-duration: 22s;
  }
  .shark:nth-child(4) {
    top: 25%;
    left: -120px;
    animation-duration: 18s;
  }
  @keyframes swim {
    0% { left: -100px; transform: scaleX(1) rotate(0deg); }
    50% { transform: scaleX(-1) rotate(10deg); }
    100% { left: 110vw; transform: scaleX(1) rotate(0deg); }
  }

  main {
    max-width: 900px;
    width: 95%;
    margin: 0 auto 50px;
    padding: 20px;
    background: rgba(0, 40, 90, 0.8);
    border-radius: 20px;
    box-shadow: 0 0 40px #00ffff80;
    color: #ccf9ff;
  }
  section {
    margin-bottom: 40px;
  }
  section h2 {
    font-size: 2.2em;
    margin-bottom: 15px;
    color: #00e5ff;
    text-shadow: 0 0 8px #00e5ff;
    text-align: center;
  }
  section p, section li {
    font-size: 1.15em;
    line-height: 1.6;
  }
  ul, ol {
    margin-left: 25px;
  }
  button {
    display: block;
    background: #00e5ff;
    border: none;
    color: #000;
    padding: 18px 50px;
    font-size: 1.3em;
    font-weight: 700;
    border-radius: 15px;
    cursor: pointer;
    box-shadow: 0 0 20px #00e5ff;
    margin: 30px auto 0 auto;
    transition: transform 0.2s ease-in-out;
  }
  button:hover {
    transform: scale(1.1);
    box-shadow: 0 0 35px #00e5ff;
  }
  a {
    color: #00ffff;
    text-decoration: underline;
  }
  .countdown {
    font-size: 2.2em;
    font-weight: 700;
    text-align: center;
    margin-top: 5px;
    margin-bottom: 30px;
    text-shadow: 0 0 12px #00ffff;
  }
  footer {
    background: #001f3f;
    color: #0088aa;
    font-size: 0.9em;
    text-align: center;
    padding: 20px 10px;
    box-shadow: inset 0 1px 3px #00ffff60;
    position: relative;
    z-index: 1000;
  }
  @media (max-width: 600px) {
    header h1 {
      font-size: 2em;
    }
    section h2 {
      font-size: 1.6em;
    }
    button {
      font-size: 1.1em;
      padding: 14px 30px;
    }
  }
</style>
</head>
<body>

<header>
  <h1>🦈 THE SHARK TOKEN</h1>
  <p>Le memecoin qui mord dans le Web3 et la blockchain Solana</p>
</header>

<!-- Requins animés -->
<img src="https://cdn.pixabay.com/animation/2023/01/18/15/18/15-18-48-185_512.gif" alt="Requin nageant" class="shark" style="top: 10%; animation-delay: 0s;"/>
<img src="https://cdn.pixabay.com/animation/2023/01/18/15/18/15-18-48-185_512.gif" alt="Requin nageant" class="shark" style="top: 40%; animation-delay: 5s;"/>
<img src="https://cdn.pixabay.com/animation/2023/01/18/15/18/15-18-48-185_512.gif" alt="Requin nageant" class="shark" style="top: 75%; animation-delay: 10s;"/>
<img src="https://cdn.pixabay.com/animation/2023/01/18/15/18/15-18-48-185_512.gif" alt="Requin nageant" class="shark" style="top: 25%; animation-delay: 15s;"/>

<main>

<section>
  <h2>⏳ Compte à rebours jusqu'au lancement</h2>
  <div id="countdown" class="countdown">Chargement...</div>
</section>

<section>
  <h2>⚒️ Minage à 0.001 SOL</h2>
  <p>Payez 0.001 SOL pour démarrer le minage et recevoir un lot de SHARK tokens automatiquement envoyés sur votre wallet.</p>
  <button id="mineBtn">Commencer le minage</button>
</section>

<section>
  <h2>📜 Whitepaper & Présentation</h2>
  <p><strong>THE SHARK TOKEN — Le memecoin qui mord dans le Web3</strong></p>
  <p>THE SHARK TOKEN est bien plus qu’un simple memecoin. Né dans les profondeurs de la blockchain Solana, il combine l’univers fun des tokens communautaires avec une utilité réelle, une vision décentralisée, et une mascotte inoubliable : le requin furieux du Web3.</p>
  <p>Rejoignez une aventure unique qui vise à :</p>
  <ul>
    <li>Récompenser les holders grâce à un système de minage innovant 🪙</li>
    <li>Permettre d’acheter et d’échanger d'autres memecoins sur une plateforme dédiée 🔁</li>
    <li>Mettre en avant la sécurité, la transparence et l’humour crypto 😎</li>
    <li>Construire une gouvernance communautaire participative 🗳️</li>
  </ul>
  <p>🌊 Explorez un univers visuel immersif : requins animés, éclairs néon, ambiance Web3.</p>
  <p>🚀 Que vous soyez un degen, un trader ou un simple curieux : rejoignez la meute ! Ne soyez pas la proie.</p>
</section>

<section>
  <h2>📅 Roadmap — Les 10 étapes clés</h2>
  <ol>
    <li>Lancement du token SHARK, création de Telegram & Twitter</li>
    <li>Première distribution + début du minage</li>
    <li>Lancement du site officiel</li>
    <li>Développement de la plateforme d’échange de memecoins</li>
    <li>Intégration de la gouvernance décentralisée</li>
    <li>Lancement de l’application mobile SHARK</li>
    <li>Campagnes marketing, giveaways & influenceurs</li>
    <li>Lancement de la collection NFT SHARK</li>
    <li>Extension multi-blockchain</li>
    <li>Création d’un fonds communautaire pour les projets votés</li>
  </ol>
</section>

<section>
  <h2>📊 Tokenomics</h2>
  <p><strong>Nom :</strong> THE SHARK TOKEN<br />
  <strong>Symbole :</strong> SHARK<br />
  <strong>Blockchain :</strong> Solana<br />
  <strong>Supply :</strong> 1,000,000,000 SHARK</p>
  <ul>
    <li>50% holders</li>
    <li>20% développement</li>
    <li>10% marketing</li>
    <li>10% réserve</li>
    <li>10% communauté</li>
  </ul>
</section>

<section>
  <h2>🔗 Liens officiels</h2>
  <p><a href="https://x.com/TheSharkTokens?t=K-Gwpm-heo5Zi93sQ1qJvg&s=09" target="_blank" rel="noopener">Twitter (X)</a></p>
  <p><a href="https://t.me/TheSharkTokenOfficial" target="_blank" rel="noopener">Telegram</a></p>
</section>

</main>

<footer>
  © 2025 THE SHARK TOKEN. Tous droits réservés.
</footer>

<script>
  // Compte à rebours
  const countdownEl = document.getElementById('countdown');
  const launchDate = new Date('2025-09-10T00:00:00').getTime();

  setInterval(() => {
    const now = new Date().getTime();
    const distance = launchDate - now;

    if (distance < 0) {
      countdownEl.innerText = "Le token est lancé !";
      return;
    }

    const days = Math.floor(distance / (1000*60*60*24));
    const hours = Math.floor((distance % (1000*60*60*24)) / (1000*60*60));
    const minutes = Math.floor((distance % (1000*60*60)) / (1000*60));
    const seconds = Math.floor((distance % (1000*60)) / 1000);

    countdownEl.innerText = `${days}j ${hours}h ${minutes}m ${seconds}s`;
  }, 1000);

  // Placeholder minage + wallet connect
  document.getElementById('mineBtn').addEventListener('click', () => {
    alert('Minage à 0.001 SOL - Intégration WalletConnect Solana à venir !');
  });
</script>

</body>
</html><nav>
  <ul>
    <li><a href="index.html">Accueil</a></li>
    <li><a href="minage.html">Minage</a></li>
    <li><a href="boutique.html">Boutique</a></li>
    <li><a href="nft.html">NFT</a></li>
    <li><a href="plateforme.html">Plateforme</a></li>
  </ul>
</nav><!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Minage - THE SHARK TOKEN</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Orbitron&display=swap');
    body {
      background: linear-gradient(to bottom, #001f3f, #004e92);
      color: #00ffff;
      font-family: 'Orbitron', sans-serif;
      text-align: center;
      padding: 40px 20px;
      min-height: 100vh;
      margin: 0;
      display: flex;
      flex-direction: column;
      justify-content: start;
      align-items: center;
    }
    h1 {
      font-size: 3em;
      margin-bottom: 10px;
      text-shadow: 0 0 12px #00ffff;
    }
    p {
      font-size: 1.3em;
      max-width: 600px;
      margin: 10px auto 30px auto;
      line-height: 1.5;
    }
    button {
      background: #00e5ff;
      border: none;
      color: #000;
      padding: 18px 50px;
      font-size: 1.4em;
      font-weight: 700;
      border-radius: 15px;
      cursor: pointer;
      box-shadow: 0 0 25px #00e5ff;
      margin: 15px;
      transition: transform 0.2s ease-in-out;
    }
    button:hover {
      transform: scale(1.1);
      box-shadow: 0 0 40px #00e5ff;
    }
    #status {
      margin-top: 30px;
      font-size: 1.2em;
      min-height: 40px;
      font-weight: 600;
      text-shadow: 0 0 8px #00ffff;
    }
    footer {
      margin-top: auto;
      padding: 15px 10px;
      color: #0088aa;
      font-size: 0.9em;
      text-align: center;
    }
    .wallet-address {
      font-family: monospace;
      background: #003366;
      padding: 8px 12px;
      border-radius: 10px;
      display: inline-block;
      margin-top: 5px;
      user-select: all;
      box-shadow: 0 0 15px #00ffff70;
    }
    .nft-info {
      margin-top: 40px;
      font-size: 1.2em;
      max-width: 700px;
      color: #66ffff;
      text-shadow: 0 0 6px #33ccff;
    }
  </style>
</head>
<body>

  <h1>⚒️ Minage THE SHARK TOKEN</h1>
  <p>
    Connectez votre wallet Solana et payez <strong>0.001 SOL</strong> pour démarrer le minage.<br />
    Un lot de SHARK tokens vous sera automatiquement envoyé sur votre wallet.
  </p>
  <p>
    <strong>Adresse de paiement (wallet réception) :</strong><br />
    <span class="wallet-address">3FbH3mmc4K4rbTaS5bbF5fhKU1EUnFEzww1ieFw6fNpE</span>
  </p>

  <button id="connectWalletBtn">Connecter Wallet</button>
  <button id="startMiningBtn" disabled>Commencer le minage</button>

  <div id="status"></div>

  <div class="nft-info">
    🚀 <strong>Futurs NFTs SHARK</strong><br />
    Préparez-vous à collectionner bientôt des NFTs exclusifs THE SHARK TOKEN.<br />
    Chaque NFT offrira des avantages uniques, accès VIP et récompenses spéciales dans l’écosystème.
  </div>

  <footer>© 2025 THE SHARK TOKEN</footer>

  <script>
    const connectWalletBtn = document.getElementById('connectWalletBtn');
    const startMiningBtn = document.getElementById('startMiningBtn');
    const statusDiv = document.getElementById('status');

    let walletConnected = false;

    connectWalletBtn.onclick = async () => {
      statusDiv.textContent = 'Connexion au wallet...';
      // Simule la connexion wallet (à remplacer par vraie intégration Wallet Adapter Solana)
      setTimeout(() => {
        walletConnected = true;
        statusDiv.textContent = 'Wallet connecté ! Vous pouvez commencer le minage.';
        startMiningBtn.disabled = false;
        connectWalletBtn.disabled = true;
      }, 1500);
    };

    startMiningBtn.onclick = async () => {
      if (!walletConnected) {
        statusDiv.textContent = 'Connectez d’abord votre wallet.';
        return;
      }
      statusDiv.textContent = 'Transaction de minage en cours...';

      // Ici, tu dois implémenter l'envoi réel de 0.001 SOL vers le wallet 3FbH3mmc4K4rbTaS5bbF5fhKU1EUnFEzww1ieFw6fNpE
      // Simulation d’attente et succès
      setTimeout(() => {
        statusDiv.textContent = 'Minage réussi ! Les SHARK tokens ont été envoyés à votre wallet.';
        startMiningBtn.disabled = true;
      }, 3000);
    };
  </script>

</body>
</html><nav>
  <ul>
    <li><a href="index.html">Accueil</a></li>
    <li><a href="minage.html">Minage</a></li>
    <li><a href="boutique.html">Boutique</a></li>
    <li><a href="nft.html">NFT</a></li>
    <li><a href="plateforme.html">Plateforme</a></li>
  </ul>
</nav><!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Boutique & Merch - THE SHARK TOKEN</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Orbitron&display=swap');
    body {
      background: linear-gradient(to bottom, #001f3f, #004e92);
      color: #00ffff;
      font-family: 'Orbitron', sans-serif;
      text-align: center;
      padding: 40px 20px;
      min-height: 100vh;
      margin: 0;
      display: flex;
      flex-direction: column;
      justify-content: start;
      align-items: center;
    }
    h1 {
      font-size: 3em;
      margin-bottom: 10px;
      text-shadow: 0 0 12px #00ffff;
    }
    p {
      font-size: 1.3em;
      max-width: 700px;
      margin: 10px auto 30px auto;
      line-height: 1.5;
    }
    .merch-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 30px;
      max-width: 900px;
    }
    .item {
      background: rgba(0, 40, 90, 0.8);
      border-radius: 20px;
      box-shadow: 0 0 25px #00e5ff80;
      padding: 20px;
      width: 250px;
      color: #ccf9ff;
      transition: transform 0.3s ease;
    }
    .item:hover {
      transform: scale(1.05);
      box-shadow: 0 0 45px #00ffff;
    }
    .item img {
      width: 100%;
      border-radius: 15px;
      margin-bottom: 15px;
      box-shadow: 0 0 15px #00e5ff;
    }
    .item h3 {
      margin: 0 0 10px 0;
      font-size: 1.5em;
      color: #00e5ff;
      text-shadow: 0 0 8px #00e5ff;
    }
    .item p {
      font-size: 1em;
      margin-bottom: 10px;
    }
    .item button {
      background: #00e5ff;
      border: none;
      color: #000;
      padding: 12px 25px;
      font-weight: 700;
      border-radius: 12px;
      cursor: pointer;
      box-shadow: 0 0 15px #00e5ff;
      font-size: 1em;
      transition: background 0.3s ease;
    }
    .item button:hover {
      background: #00b8cc;
    }
    footer {
      margin-top: auto;
      padding: 15px 10px;
      color: #0088aa;
      font-size: 0.9em;
      text-align: center;
    }
  </style>
</head>
<body>

  <h1>🛒 Boutique & Merch THE SHARK TOKEN</h1>

  <p>
    Découvrez bientôt notre boutique officielle avec des articles exclusifs THE SHARK TOKEN.<br />
    Montrez votre appartenance à la meute avec style grâce à notre merch : t-shirts, casquettes, stickers et plus.<br />
    Les paiements pourront être réalisés en SHARK tokens ou SOL via notre plateforme Web3 sécurisée.
  </p>

  <div class="merch-list">
    <div class="item">
      <img src="https://i.imgur.com/JrTfwQw.png" alt="T-shirt Shark Token" />
      <h3>T-shirt Shark Token</h3>
      <p>Confort premium avec logo THE SHARK TOKEN néon. Disponible en plusieurs tailles.</p>
      <button>Acheter en SHARK</button>
    </div>
    <div class="item">
      <img src="https://i.imgur.com/8y6B9uE.png" alt="Casquette Shark Token" />
      <h3>Casquette Shark Token</h3>
      <p>Casquette stylée pour compléter ton look Web3. Logo brodé bleu néon.</p>
      <button>Acheter en SHARK</button>
    </div>
    <div class="item">
      <img src="https://i.imgur.com/ykDc9Oq.png" alt="Sticker Shark Token" />
      <h3>Sticker Shark Token</h3>
      <p>Autocollants vinyl waterproof parfaits pour personnaliser ton matos crypto.</p>
      <button>Acheter en SHARK</button>
    </div>
  </div>

  <section style="margin-top: 50px; max-width: 700px; color: #66ffff; text-shadow: 0 0 6px #33ccff; font-size: 1.2em;">
    <h2>🔮 Futurs développements & prédictions</h2>
    <p>
      THE SHARK TOKEN vise à devenir un acteur clé du Web3 sur Solana.<br />
      Voici quelques prédictions réalistes pour les prochains mois :
    </p>
    <ul style="text-align: left; max-width: 500px; margin: auto; list-style-type: disc; padding-left: 20px;">
      <li>Lancement réussi de la plateforme d’échange de memecoins intégrée.</li>
      <li>Expansion de la communauté avec +100,000 holders actifs.</li>
      <li>Développement de la collection NFT SHARK avec utilité réelle.</li>
      <li>Intégration multi-blockchain pour plus de liquidité.</li>
      <li>Campagnes marketing fortes pour booster la visibilité.</li>
      <li>Partenariats avec projets DeFi et gaming Web3.</li>
    </ul>
    <p>Le tout avec une gouvernance communautaire solide et une transparence totale pour assurer la confiance des investisseurs.</p>
  </section>

  <footer>© 2025 THE SHARK TOKEN</footer>

</body>
</html><nav>
  <ul>
    <li><a href="index.html">Accueil</a></li>
    <li><a href="minage.html">Minage</a></li>
    <li><a href="boutique.html">Boutique</a></li>
    <li><a href="nft.html">NFT</a></li>
    <li><a href="plateforme.html">Plateforme</a></li>
  </ul>
</nav><!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Future plateforme d’échange - THE SHARK TOKEN</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Orbitron&display=swap');
    body {
      background: linear-gradient(to bottom, #001f3f, #004e92);
      color: #00ffff;
      font-family: 'Orbitron', sans-serif;
      text-align: center;
      padding: 50px 20px;
      min-height: 100vh;
      margin: 0;
      display: flex;
      flex-direction: column;
      justify-content: start;
      align-items: center;
    }
    h1 {
      font-size: 3.2em;
      margin-bottom: 20px;
      text-shadow: 0 0 15px #00ffff;
    }
    p {
      font-size: 1.4em;
      max-width: 700px;
      margin: 0 auto 40px auto;
      line-height: 1.6;
    }
    ul {
      text-align: left;
      max-width: 650px;
      list-style-type: disc;
      padding-left: 25px;
      font-size: 1.2em;
      margin-bottom: 40px;
    }
    ul li {
      margin-bottom: 15px;
    }
    footer {
      margin-top: auto;
      padding: 15px 10px;
      color: #0088aa;
      font-size: 0.9em;
      text-align: center;
    }
    .highlight {
      color: #33ffff;
      font-weight: 700;
      text-shadow: 0 0 8px #33ffff;
    }
  </style>
</head>
<body>

  <h1>🔗 Future plateforme d’échange de memecoins</h1>

  <p>
    Si THE SHARK TOKEN continue sa croissance et sa réussite, nous envisageons de lancer une plateforme décentralisée d’échange dédiée aux memecoins sur Solana.<br /><br />
    Cette plateforme offrira aux utilisateurs la possibilité d’acheter, vendre et échanger facilement une sélection rigoureuse de memecoins, dans un environnement sécurisé, rapide et communautaire.
  </p>

  <h2 class="highlight">Fonctionnalités clés prévues :</h2>
  <ul>
    <li>Interface intuitive et responsive, adaptée mobile et desktop.</li>
    <li>Intégration native des wallets Solana (Phantom, Solflare, etc.).</li>
    <li>Échanges rapides avec faibles frais de transaction grâce à Solana.</li>
    <li>Sélection rigoureuse des memecoins listés, avec validation communautaire.</li>
    <li>Programme de récompenses pour les utilisateurs actifs et holders.</li>
    <li>Fonctionnalités de gouvernance pour que la communauté décide des évolutions.</li>
    <li>Transparence totale avec code open-source et audits réguliers.</li>
  </ul>

  <p>
    Cette plateforme vise à devenir un hub central du Web3 memecoin, facilitant l’accès, la sécurité et l’amusement pour tous les passionnés.<br />
    Rejoignez-nous dès maintenant pour faire partie de cette aventure révolutionnaire !
  </p>

  <footer>© 2025 THE SHARK TOKEN</footer>

</body>
</html><nav>
  <ul>
    <li><a href="index.html">Accueil</a></li>
    <li><a href="minage.html">Minage</a></li>
    <li><a href="boutique.html">Boutique</a></li>
    <li><a href="nft.html">NFT</a></li>
    <li><a href="plateforme.html">Plateforme</a></li>
  </ul>
</nav>