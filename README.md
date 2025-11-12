# Site-do-flamengo
Um site do flamengo feito por fan mas con informações originais
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Flamengo - Clube de Regatas</title>
  <style>
    :root {
      --red: #e10600;
      --black: #000;
      --white: #fff;
    }
    body {
      margin: 0;
      font-family: "Inter", system-ui, Arial, sans-serif;
      background: #fff;
      color: #111;
    }
    header {
      background: var(--black);
      color: var(--white);
      padding: 15px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    header img.logo {
      height: 50px;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 25px;
      margin: 0;
      padding: 0;
    }
    nav ul li a {
      color: var(--white);
      text-decoration: none;
      font-weight: 600;
    }
    .hero {
      background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('assets/hero-flamengo.jpg') center/cover no-repeat;
      height: 60vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 0 40px;
      color: var(--white);
    }
    .hero h1 {
      font-size: 3.5rem;
      margin: 0 0 15px 0;
    }
    .hero p {
      font-size: 1.3rem;
      max-width: 500px;
      margin-bottom: 20px;
    }
    .hero a.cta {
      background: var(--red);
      color: var(--white);
      padding: 12px 28px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: 700;
      width: max-content;
    }
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
      gap: 20px;
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
    }
    .card {
      background: #fafafa;
      border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      overflow: hidden;
      text-align: left;
    }
    .card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      display: block;
    }
    .card h3 {
      margin: 12px 16px 6px 16px;
      font-size: 1.2rem;
    }
    .card p {
      margin: 0 16px 16px 16px;
      color: #555;
      font-size: 0.95rem;
    }
    footer {
      background: var(--black);
      color: var(--white);
      padding: 18px 20px;
      text-align: center;
    }
    footer a {
      color: var(--white);
      margin: 0 12px;
      text-decoration: none;
    }
    @media(max-width: 600px) {
      .hero h1 {
        font-size: 2.5rem;
      }
      .hero p {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <img src="assets/logo-flamengo.png" alt="Logo do Flamengo" class="logo" />
    <nav aria-label="Menu principal">
      <ul>
        <li><a href="index.html">Início</a></li>
        <li><a href="historia.html">História</a></li>
        <li><a href="elenco.html">Elenco</a></li>
        <li><a href="conquistas.html">Conquistas</a></li>
        <li><a href="calendario.html">Calendário</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero" aria-label="Destaque principal do Flamengo">
    <h1>Clube de Regatas do Flamengo</h1>
    <p>Fundado em 1895, o Flamengo é o clube mais popular do Brasil, com uma rica história de conquistas nacionais e internacionais.</p>
    <a href="calendario.html" class="cta">Confira o próximo jogo</a>
  </section>

  <section class="cards" aria-label="Seções principais do site">
    <article class="card">
      <img src="assets/historia.jpg" alt="História do Flamengo" />
      <h3>Nossa História</h3>
      <p>Descubra como tudo começou e os principais marcos que moldaram o clube.</p>
    </article>
    <article class="card">
      <img src="assets/elenco.jpg" alt="Elenco do Flamengo" />
      <h3>Elenco Atual</h3>
      <p>Conheça os jogadores que representam nosso time em campo.</p>
    </article>
    <article class="card">
      <img src="assets/conquistas.jpg" alt="Trofeus do Flamengo" />
      <h3>Conquistas</h3>
      <p>Explore os títulos importantes conquistados ao longo dos anos.</p>
    </article>
  </section>

  <footer>
    <p>© Clube de Regatas do Flamengo. Todos os direitos reservados.</p>
    <a href="#" aria-label="Instagram">Instagram</a>|
    <a href="#" aria-label="YouTube">YouTube</a>|
    <a href="#" aria-label="Twitter">X</a>
  </footer>
</body>
</html>
