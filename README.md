<html lang="bs">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CoreLogic | IT Usluge</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: linear-gradient(135deg, #6a0dad, #a85dd7);
      color: white;
      scroll-behavior: smooth;
    }
    header {
      text-align: center;
      padding: 100px 20px 40px;
      animation: fadeIn 1.2s ease-in-out;
    }
    .logo {
      width: 300px;
      height: auto;
      margin-bottom: 30px;
    }
    header h1 {
      font-size: 4em;
      margin-bottom: 10px;
    }
    header p {
      font-size: 1.3em;
      max-width: 700px;
      margin: 0 auto;
    }
    section {
      padding: 60px 20px;
      max-width: 1200px;
      margin: 0 auto;
    }
    h2 {
      text-align: center;
      font-size: 2.5em;
      margin-bottom: 40px;
    }
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }
    .service {
      background: rgba(255,255,255,0.1);
      border-radius: 16px;
      padding: 30px;
      text-align: center;
      transition: transform 0.3s ease, background 0.3s ease;
      backdrop-filter: blur(10px);
      cursor: pointer;
    }
    .service:hover {
      transform: translateY(-8px);
      background: rgba(255,255,255,0.15);
    }
    .service img {
      width: 50px;
      margin-bottom: 20px;
    }
    .service-detail {
      display: none;
      padding-top: 10px;
      font-size: 0.95em;
      color: #f0f0f0;
    }
    .service.open .service-detail {
      display: block;
    }
    .comment-form {
      margin-top: 60px;
      background: rgba(255,255,255,0.1);
      padding: 30px;
      border-radius: 16px;
    }
    .comment-form textarea, .comment-form input {
      width: 100%;
      padding: 12px;
      border: none;
      border-radius: 8px;
      margin-top: 10px;
      font-family: inherit;
    }
    .comment-form button {
      margin-top: 15px;
      padding: 12px 24px;
      border: none;
      background-color: #fff;
      color: #6a0dad;
      font-weight: bold;
      border-radius: 8px;
      cursor: pointer;
    }
    .comment-form button:hover {
      background-color: #eee;
    }
    footer {
      text-align: center;
      padding: 40px 20px;
      background: rgba(0, 0, 0, 0.2);
      border-top: 1px solid rgba(255, 255, 255, 0.2);
    }
    footer a {
      color: #fff;
      text-decoration: none;
      margin: 0 10px;
    }
    footer a:hover {
      text-decoration: underline;
    }
    @keyframes fadeIn {
      from {opacity: 0; transform: translateY(-20px);}
      to {opacity: 1; transform: translateY(0);}
    }
  </style>
  <script>
    function toggleDetail(index) {
      const cards = document.querySelectorAll('.service');
      cards[index].classList.toggle('open');
    }
  </script>
</head>
<body>
  <header>
    <img src="CoreLogiccc.png" alt="CoreLogic logo" class="logo">
    <h1>CoreLogic</h1>
    <p>Profesionalne IT usluge: dizajn, razvoj, dokumenti i video editing – sve na jednom mjestu.</p>
  </header>

  <section>
    <h2>Usluge koje nudimo</h2>
    <div class="services">
      <div class="service" onclick="toggleDetail(0)">
        <img src="https://cdn-icons-png.flaticon.com/512/1828/1828884.png" alt="Logo dizajn">
        <h3>Kreiranje logotipa</h3>
        <div class="service-detail">Profesionalni i moderni logotipi prilagođeni vašem brendu. Primjeri dostupni na upit.</div>
      </div>
      <div class="service" onclick="toggleDetail(1)">
        <img src="https://cdn-icons-png.flaticon.com/512/3062/3062634.png" alt="Posteri i dizajn">
        <h3>Posteri & Dizajn</h3>
        <div class="service-detail">Kreativna grafika za događaje, promocije i digitalne kampanje.</div>
      </div>
      <div class="service" onclick="toggleDetail(2)">
        <img src="https://cdn-icons-png.flaticon.com/512/1087/1087815.png" alt="Web stranice">
        <h3>Web stranice</h3>
        <div class="service-detail">Responsivne, brze i vizuelno privlačne stranice. Primjeri: portfolio, firme, restorani...</div>
      </div>
      <div class="service" onclick="toggleDetail(3)">
        <img src="https://cdn-icons-png.flaticon.com/512/2933/2933245.png" alt="Maturski radovi">
        <h3>Maturski radovi</h3>
        <div class="service-detail">Pomoć u izradi i oblikovanju maturskih i seminarskih radova.</div>
      </div>
      <div class="service" onclick="toggleDetail(4)">
        <img src="https://cdn-icons-png.flaticon.com/512/1160/1160358.png" alt="Video editing">
        <h3>Video Editing</h3>
        <div class="service-detail">Montaža, efekti i obrada videa za YouTube, društvene mreže i reklame.</div>
      </div>
      <div class="service" onclick="toggleDetail(5)">
        <img src="https://cdn-icons-png.flaticon.com/512/888/888879.png" alt="Office dokumenti">
        <h3>Word / Excel / PowerPoint</h3>
        <div class="service-detail">Obrada, dizajn i uređivanje dokumenata i tabela.</div>
      </div>
      <div class="service" onclick="toggleDetail(6)">
        <img src="https://cdn-icons-png.flaticon.com/512/3059/3059987.png" alt="QR kodovi">
        <h3>QR Kodovi</h3>
        <div class="service-detail">Generisanje personalizovanih QR kodova za sve potrebe.</div>
      </div>
    </div>
  </section>

  <section class="comment-form">
    <h2>Ostavite komentar</h2>
    <form action="#" method="post">
      <input type="text" name="ime" placeholder="Vaše ime" required>
      <textarea name="komentar" placeholder="Vaš komentar..." rows="5" required></textarea>
      <button type="submit">Pošalji</button>
    </form>
  </section>

  <footer>
    <p>Kontaktirajte nas:</p>
    <a href="mailto:ccorelogicc@gmail.com">
      <img src="https://cdn-icons-png.flaticon.com/512/732/732200.png" alt="Gmail" width="20" style="vertical-align: middle;"> ccorelogicc@gmail.com
    </a>
    |
    <a href="https://instagram.com/coreelogic" target="_blank">
      <img src="https://cdn-icons-png.flaticon.com/512/174/174855.png" alt="Instagram" width="20" style="vertical-align: middle;"> @coreelogic
    </a>
    <p style="margin-top: 20px; font-size: 0.9em; color: #ddd;">© 2025 CoreLogic. Sva prava zadržana.</p>
  </footer>
</body>
</html>
