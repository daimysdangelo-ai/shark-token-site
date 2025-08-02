# shark-token-site
site officiel de The Shark TOKEN - Projet Web3 base sur Solana
dede, [02/08/2025 10:45]
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Shark Token - Accueil</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <header class="hero">
    <img src="assets/logo-shark.png" alt="Shark Token Logo" class="logo">
    <h1>Bienvenue dans l’océan du Web3</h1>
    <p class="tagline">The Shark Token débarque. Un projet communautaire sur Solana, puissant et déterminé à s’imposer.</p>
    <div class="cta">
      <a href="https://discord.gg/tonlien" class="btn">Rejoindre Discord</a>
      <a href="whitepaper.html" class="btn-secondary">Lire le Whitepaper</a>
    </div>
  </header>

  <section class="about">
    <h2>Qui sommes-nous ?</h2>
    <p>
      The Shark Token (SHARK) est un token communautaire lancé sur Solana. Inspiré du requin – symbole ultime de domination, agilité et instinct.
    </p>
    <ul>
      <li>✔️ Identité forte & cohérente</li>
      <li>✔️ Communauté engagée</li>
      <li>✔️ Futur : Staking, NFT, DAO</li>
    </ul>
  </section>

  <section class="tokenomics">
    <h2>📊 Tokenomics</h2>
    <table>
      <tr><td>Supply totale</td><td>1 000 000 000 SHARK</td></tr>
      <tr><td>Prévente</td><td>20%</td></tr>
      <tr><td>Liquidity Pool</td><td>40%</td></tr>
      <tr><td>Développement</td><td>15%</td></tr>
      <tr><td>Marketing / Partenaires</td><td>15%</td></tr>
      <tr><td>Airdrop / Communauté</td><td>10%</td></tr>
      <tr><td>Liquidité verrouillée</td><td>Oui – X mois</td></tr>
      <tr><td>Anti-bot / farm</td><td>Oui – mécanique intégrée</td></tr>
    </table>
  </section>

  <section class="roadmap">
    <h2>🛣️ Roadmap</h2>
    <div class="phase">
      <h3>✅ Phase 1 – Lancement</h3>
      <ul>
        <li>✔️ Création du token</li>
        <li>✔️ Branding visuel</li>
        <li>✔️ Lancement de la communauté</li>
      </ul>
    </div>
    <div class="phase">
      <h3>🔜 Phase 2 – Croissance</h3>
      <ul>
        <li>📄 Publication du Whitepaper</li>
        <li>🎁 Airdrops & concours</li>
        <li>🧬 Développement d’utilités (staking, NFT)</li>
      </ul>
    </div>
    <div class="phase">
      <h3>🚀 Phase 3 – Transformation</h3>
      <ul>
        <li>📈 Listing sur DEX</li>
        <li>🗳️ Lancement de la DAO</li>
        <li>🌐 Mini apps & outils communautaires Web3</li>
      </ul>
    </div>
  </section>

  <section class="community">
    <h2>🌍 Rejoins la communauté</h2>
    <p>
      Twitter (X) : <a href="https://x.com/TheSharkToken">@TheSharkToken</a> <br>
      Telegram : <a href="https://t.me/SharkToken">t.me/SharkToken</a> <br>
      Discord : <a href="https://discord.gg/tonlien">Lien Discord</a>
    </p>
  </section>

  <footer>
    <p>⚠️ Ce site ne constitue pas un conseil financier.</p>
    <p>Chain : Solana – SPL Token – vérifiez toujours l’adresse !</p>
    <p>© 2025 The Shark Token. Tous droits réservés. Contact : team@sharktoken.xyz</p>
  </footer>

</body>
</html>

dede, [02/08/2025 10:45]
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: #0d1117;
  color: #f0f0f0;
}

.hero {
  text-align: center;
  padding: 60px 20px;
  background: linear-gradient(to right, #0d1117, #1f2937);
}

.logo {
  width: 120px;
  margin-bottom: 20px;
}

.tagline {
  font-size: 1.2em;
  max-width: 600px;
  margin: auto;
}

.cta {
  margin-top: 30px;
}

.btn, .btn-secondary {
  display: inline-block;
  margin: 10px;
  padding: 12px 24px;
  border-radius: 6px;
  font-weight: bold;
  text-decoration: none;
}

.btn {
  background-color: #1e90ff;
  color: white;
}

.btn-secondary {
  border: 2px solid #1e90ff;
  color: #1e90ff;
}

section {
  padding: 40px 20px;
  max-width: 900px;
  margin: auto;
}

h2 {
  color: #58a6ff;
}

table {
  width: 100%;
  border-collapse: collapse;
  background-color: #161b22;
  border-radius: 8px;
  overflow: hidden;
}

td {
  padding: 12px;
  border-bottom: 1px solid #30363d;
}

.phase {
  margin-top: 30px;
  background-color: #161b22;
  padding: 20px;
  border-radius: 8px;
}

a {
  color: #58a6ff;
}

footer {
  text-align: center;
  padding: 30px;
  font-size: 0.9em;
  background-color: #161b22;
  margin-top: 50px;
}

dede, [02/08/2025 10:45]
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>The Shark Token – Vision & Whitepaper</title>
  <link rel="stylesheet" href="style.css">
  <style>
    .accordion {
      background-color: #161b22;
      color: white;
      cursor: pointer;
      padding: 15px;
      border: none;
      text-align: left;
      outline: none;
      transition: 0.3s;
      font-size: 1em;
      margin-bottom: 5px;
    }
    .accordion.active, .accordion:hover {
      background-color: #1f2937;
    }
    .panel {
      padding: 0 15px;
      display: none;
      background-color: #0d1117;
      overflow: hidden;
    }
  </style>
</head>
<body>

  <header class="hero">
    <img src="assets/logo-shark.png" alt="Shark Token Logo" class="logo">
    <h1>Whitepaper & Vision</h1>
    <p class="tagline">The Shark Token – Plus qu’un token, une transformation.</p>
    <a href="index.html" class="btn-secondary">⬅️ Retour à l’accueil</a>
  </header>

  <section>
    <h2>🧬 Utilité & Vision long terme</h2>
    <p>
      SHARK est conçu pour évoluer avec le temps. Chaque étape de croissance débloque de nouvelles fonctionnalités. Comme un requin, notre token devient plus fort à chaque transformation.
    </p>
    <ul>
      <li>🔹 <strong>Staking</strong> – Gagne des récompenses en bloquant tes SHARK</li>
      <li>🔹 <strong>NFT</strong> – Collectionne des requins évolutifs avec raretés</li>
      <li>🔹 <strong>DAO</strong> – Prends des décisions avec la communauté</li>
      <li>🔹 <strong>DApps</strong> – Expériences interactives Web3 pour holders</li>
    </ul>
  </section>

  <section>
    <h2>🦈 Évolution du projet</h2>
    <p>
      Le Shark Token n’est pas statique. Il passe par 3 stades d’évolution :
    </p>
    <ul>
      <li><strong>Phase Bébé Requin</strong> 🐟 – Naissance du projet, branding, croissance organique</li>
      <li><strong>Phase Requin Alpha</strong> 🦈 – Utilité, écosystème, airdrops, outils communautaires</li>
      <li><strong>Phase SharkDAO</strong> 👑 – Gouvernance décentralisée, apps Web3, pouvoir au peuple</li>
    </ul>
  </section>

  <section>
    <h2>📖 Contenu du Whitepaper</h2>
    <p>
      👉 <strong>Télécharger le PDF</strong> : <a href="#">(à héberger)</a>
    </p>
    <ul>
      <li>1. Présentation & Origine</li>
      <li>2. Tokenomics & Sécurité</li>
      <li>3. Roadmap & Objectifs</li>
      <li>4. Équipe & Gouvernance</li>
      <li>5. Risques & transparence</li>
    </ul>
  </section>

  <section>
    <h2>❓ FAQ</h2>
    <button class="accordion">Le SHARK Token est-il certifié ?</button>
    <div class="panel"><p>Oui, le smart contract est vérifiable sur Solana (SPL Token). Audit prévu Phase 2.</p></div>

    <button class="accordion">Peut-on déjà acheter le token ?</button>
    <div class="panel"><p>Pas encore. Prévente à venir dans la roadmap Phase 1.</p></div>

    <button class="accordion">Comment participer à la DAO ?</button>
    <div class="panel"><p>Les holders de SHARK recevront des droits de vote une fois la DAO lancée (Phase 3).</p></div>
  </section>

  <footer>
    <p>⚠️ Ceci n'est pas un conseil financier. Investissez en connaissance de cause.</p>
    <p>© 2025 The Shark Token – Projet Solana</p>
  </footer>

  <script>
    const acc = document.getElementsByClassName("accordion");
    for (let i = 0; i < acc.length; i++) {
      acc[i].addEventListener("click", function () {
        this.classList.toggle("active");
        const panel = this.nextElementSibling;
        panel.style.display = panel.style.display === "block" ? "none" : "block";
      });
    }
  </script>

</body>
</html>
