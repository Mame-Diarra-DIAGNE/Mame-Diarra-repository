<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Boxe & Bien-Être</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #1E2B45;
      color: white;
      line-height: 1.6;
    }

    header {
      background-color: #D8A641;
      color: #1E2B45;
      padding: 1rem;
      text-align: center;
    }

    nav {
      display: flex;
      justify-content: flex-end;
      background-color: #1E2B45;
      padding: 0.5rem 1rem;
      gap: 1rem;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      border: 1px solid #D8A641;
      padding: 0.4rem 0.8rem;
      border-radius: 5px;
      transition: background 0.3s;
    }

    nav a:hover {
      background-color: #D8A641;
      color: #1E2B45;
    }

    .section {
      padding: 2rem;
      border-bottom: 1px solid #D8A641;
    }

    h2 {
      color: #D8A641;
    }

    .grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 2rem;
      align-items: center;
    }

    .grid img {
      width: 100%;
      border-radius: 10px;
    }

    footer {
      background-color: #D8A641;
      color: #1E2B45;
      text-align: center;
      padding: 1rem;
    }

    @media (max-width: 768px) {
      .grid {
        grid-template-columns: 1fr;
      }

      nav {
        flex-direction: column;
        align-items: flex-end;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Boxe & Bien-Être</h1>
    <p>Découvrez la boxe autrement, sans salle et sans sac <br />
  </header>

  <nav>
    <a href="#inscription">Inscription</a>
    <a href="#connexion">Connexion</a>
    <a href="#reserver">Réserver</a>
    <button onclick="toggleLang()" id="langButton">EN</button>
    <script>
      function toggleLang() {
        const button = document.getElementById('langButton');
        if (button.textContent === 'EN') {
          button.textContent = 'FR';
          document.documentElement.lang = 'en';
        } else {
          button.textContent = 'EN';
          document.documentElement.lang = 'fr';
        }
      }
    </script>
  </nav>

  <section class="section grid">
    <div>
      <h2>Méthode</h2>
      <p>Mélange de boxe Thaï, Kung-fu et Yoga<br />
      <p>Séances dynamiques, ludiques et positives<br />
    </div>
    <img src="images/entrainement.jpg" alt="Boxe image" />
  </section>

  <section class="section grid">
    <img src="images/portrait.jpg" alt="Coach Brice" />
    <div>
      <h2>Bienfaits</h2>
      <ul>
        <li>Renforcement musculaire</li>
        <li>Cardio</li>
        <li>Confiance en soi</li>
        <li>Posture</li>
      </ul>
    </div>
  </section>

  <section class="section">
    <h2>En pratique</h2>
    <p>Solo ou Duo, tout public<br />
    <p>À domicile ou en extérieur<br />
    <p>Tarif dégressif</p>
  </section>

  <section class="section" id="reserver">
    <h2>Réserver</h2>
    <p>Contactez-nous pour réserver une séance<br />
    <!-- Placeholder bouton -->
    <button>Réserver maintenant / Book now</button>
    <h2>Contact</h2>
    <p>Téléphone / Phone: 06 08 91 67 57</p>
    <p>Email: brice.ait.sport@gmail.com</p>
    <p>Adresse : Grenoble</p>
    <a href="https://wa.me/33785631190" class="btn">WhatsApp</a>
  </section>


  <section class="section" id="inscription">
    <h2>Inscription / Sign up</h2>
    <p>Créez votre compte pour accéder aux séances<br />
    <!-- Placeholder bouton -->
    <button>S'inscrire / Sign up</button>
  </section>

  <section class="section" id="connexion">
    <h2>Connexion</h2>
    <p>Déjà inscrit ? Connectez-vous ici<br>
    <!-- Placeholder bouton -->
    <button>Se connecter / Login</button>
  </section>

  <footer>
    Coach Brice – Boxeur professionnel<br />
    Coach sportif diplômé d'État – SIRET 076790809775
  </footer>
</body>
</html>
