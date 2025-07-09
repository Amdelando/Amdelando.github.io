<!DOCTYPE html><html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NexusBM | Soluções Digitais</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #f7f8fa;
      --text: #111;
      --primary: #1a1a1a;
      --secondary: #292929;
      --light: white;
    }
    @media (prefers-color-scheme: dark) {
      :root {
        --bg: #121212;
        --text: #f1f1f1;
        --primary: #000000;
        --secondary: #1e1e1e;
        --light: #1f1f1f;
      }
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Inter', sans-serif;
      background-color: var(--bg);
      color: var(--text);
      scroll-behavior: smooth;
    }
    header {
      background: url('https://images.unsplash.com/photo-1533750516457-a7f992034fec?auto=format&fit=crop&w=1400&q=80') center/cover no-repeat;
      color: white;
      padding: 80px 20px;
      text-align: center;
      animation: fadeIn 1s ease-in-out;
    }
    header h1 {
      font-size: 3rem;
      font-weight: 800;
    }
    header p {
      font-size: 1.2rem;
      margin-top: 10px;
    }
    nav {
      background-color: var(--secondary);
      padding: 15px;
      display: flex;
      justify-content: center;
      gap: 25px;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #00d8ff;
    }
    section {
      padding: 80px 20px;
      max-width: 1200px;
      margin: auto;
      animation: fadeUp 1s ease-in-out;
    }
    .section-title {
      font-size: 2.5rem;
      margin-bottom: 30px;
      text-align: center;
    }
    .services-grid, .portfolio-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
    }
    .card {
      background: var(--light);
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.05);
      transition: transform 0.3s;
    }
    .card:hover {
      transform: translateY(-5px);
    }
    .card img {
      width: 100%;
      border-radius: 8px;
      margin-bottom: 15px;
    }
    .contact {
      background: #eaeaea;
      padding: 60px 20px;
      border-radius: 12px;
      text-align: center;
    }
    .contact form {
      display: flex;
      flex-direction: column;
      max-width: 500px;
      margin: auto;
    }
    .contact input, .contact textarea {
      padding: 12px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    .contact button {
      background-color: var(--primary);
      color: white;
      padding: 12px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }
    footer {
      background-color: var(--primary);
      color: white;
      text-align: center;
      padding: 20px;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <header>
    <h1>NexusBM</h1>
    <p>Transformando ideias em resultados digitais de verdade.</p>
  </header>  <nav>
    <a href="#sobre">Sobre</a>
    <a href="#servicos">Serviços</a>
    <a href="#portfolio">Portfólio</a>
    <a href="#contato">Contato</a>
  </nav>  <section id="sobre">
    <h2 class="section-title">Sobre Nós</h2>
    <p>A NexusBM nasceu com o propósito de impulsionar empresas e marcas por meio de soluções digitais estratégicas e criativas. Com uma equipe formada por Luiz Martins e Victor Baldez, atuamos há mais de 8 meses em gestão de tráfego pago, design, sites e muito mais.</p>
  </section>  <section id="servicos">
    <h2 class="section-title">Nossos Serviços</h2>
    <div class="services-grid">
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?marketing" alt="Gestão de Tráfego">
        <h3>Gestão de Tráfego</h3>
        <p>Campanhas estratégicas no Google e nas redes sociais para atrair clientes ideais.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?webdesign" alt="Criação de Sites">
        <h3>Criação de Sites</h3>
        <p>Sites modernos, responsivos e voltados para conversão.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?copywriting" alt="Copywriting">
        <h3>Copywriting</h3>
        <p>Textos persuasivos que aumentam o valor da sua marca e geram ação.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?graphic" alt="Design Gráfico">
        <h3>Design Gráfico</h3>
        <p>Criação de identidade visual impactante, flyers, logos e muito mais.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?technology" alt="Especialista CTO">
        <h3>Especialista CTO</h3>
        <p>Consultoria técnica e estrutura digital para projetos de alto nível.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?business" alt="Google Meu Negócio">
        <h3>Google Meu Negócio</h3>
        <p>Otimize sua presença local e conquiste mais clientes perto de você.</p>
      </div>
    </div>
  </section>  <section id="portfolio">
    <h2 class="section-title">Portfólio</h2>
    <div class="portfolio-grid">
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?website" alt="Projeto 1">
        <h3>Landing Page para Startup</h3>
        <p>Site desenvolvido com foco em captação de leads e performance.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?branding" alt="Projeto 2">
        <h3>Identidade Visual para Loja</h3>
        <p>Criação de logotipo, paleta de cores e artes promocionais.</p>
      </div>
    </div>
  </section>  <section id="contato" class="contact">
    <h2 class="section-title">Fale com a Gente</h2>
    <p>Entre em contato e leve sua marca para o próximo nível:</p>
    <form action="https://formsubmit.co/seuemail@gmail.com" method="POST">
      <input type="text" name="nome" placeholder="Seu nome" required>
      <input type="email" name="email" placeholder="Seu e-mail" required>
      <textarea name="mensagem" rows="5" placeholder="Sua mensagem" required></textarea>
      <button type="submit">Enviar Mensagem</button>
    </form>
  </section>  <footer>
    <p>&copy; 2025 NexusBM — Todos os direitos reservados.</p>
  </footer>
</body>
</html>