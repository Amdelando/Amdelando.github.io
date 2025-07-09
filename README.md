<!DOCTYPE html><html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NexusBM | Soluções Digitais</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #f5f5f7;
      --text: #121212;
      --accent: #0066ff;
      --card: #ffffff;
      --dark-bg: #121212;
      --dark-text: #f5f5f7;
      --dark-card: #1e1e1e;
    }
    @media (prefers-color-scheme: dark) {
      :root {
        --bg: var(--dark-bg);
        --text: var(--dark-text);
        --card: var(--dark-card);
      }
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Inter', sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }
    header {
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      color: white;
      padding: 80px 20px;
      text-align: center;
      animation: fadeIn 1s ease-in-out;
    }
    header h1 {
      font-size: 3.2rem;
      font-weight: 800;
    }
    header p {
      margin-top: 10px;
      font-size: 1.2rem;
    }
    nav {
      background: #000;
      padding: 15px;
      display: flex;
      justify-content: center;
      gap: 30px;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s;
    }
    nav a:hover {
      color: var(--accent);
    }
    section {
      padding: 80px 20px;
      max-width: 1200px;
      margin: auto;
    }
    .section-title {
      text-align: center;
      font-size: 2.5rem;
      margin-bottom: 40px;
    }
    .services-grid, .portfolio-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
    }
    .card {
      background: var(--card);
      padding: 20px;
      border-radius: 16px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.08);
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 15px 40px rgba(0,0,0,0.1);
    }
    .card img {
      width: 100%;
      border-radius: 10px;
      margin-bottom: 15px;
    }
    .contact {
      background: linear-gradient(to right, #667eea, #764ba2);
      color: white;
      border-radius: 16px;
      padding: 60px 20px;
      text-align: center;
    }
    .contact form {
      max-width: 500px;
      margin: auto;
      display: flex;
      flex-direction: column;
    }
    .contact input, .contact textarea {
      padding: 14px;
      margin: 10px 0;
      border: none;
      border-radius: 8px;
    }
    .contact button {
      background: #000;
      color: white;
      padding: 14px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: 600;
    }
    footer {
      background: #000;
      color: white;
      padding: 20px;
      text-align: center;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <header>
    <h1>NexusBM</h1>
    <p>Transformando ideias em resultados digitais reais.</p>
  </header>  <nav>
    <a href="#sobre">Sobre</a>
    <a href="#servicos">Serviços</a>
    <a href="#portfolio">Portfólio</a>
    <a href="#contato">Contato</a>
  </nav>  <section id="sobre">
    <h2 class="section-title">Sobre Nós</h2>
    <p style="text-align: center; max-width: 800px; margin: auto;">Somos uma agência especializada em marketing digital, design e tecnologia. Há 8 meses entregamos resultados que transformam marcas e conectam empresas aos seus públicos de forma eficaz e moderna.</p>
  </section>  <section id="servicos">
    <h2 class="section-title">O que fazemos</h2>
    <div class="services-grid">
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?ads" alt="Gestão de Tráfego">
        <h3>Gestão de Tráfego Pago</h3>
        <p>Campanhas no Google, Instagram e Facebook com foco em conversão real.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?website" alt="Sites Profissionais">
        <h3>Criação de Sites</h3>
        <p>Sites rápidos, bonitos e com ótima performance para celular e desktop.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?copywriting,typing" alt="Copywriting">
        <h3>Copywriting</h3>
        <p>Textos que vendem, envolvem e criam autoridade para sua marca.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?branding" alt="Design Gráfico">
        <h3>Design Gráfico</h3>
        <p>Artes, logos e identidades visuais impactantes e memoráveis.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?technology,code" alt="CTO">
        <h3>Especialista CTO</h3>
        <p>Consultoria técnica para digitalizar seu negócio com estratégia.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?location,map" alt="Google Meu Negócio">
        <h3>Google Meu Negócio</h3>
        <p>Coloque sua empresa no mapa e apareça no Google local.</p>
      </div>
    </div>
  </section>  <section id="portfolio">
    <h2 class="section-title">Portfólio</h2>
    <div class="portfolio-grid">
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?startup" alt="Projeto 1">
        <h3>Startup Tech</h3>
        <p>Landing page responsiva com foco em captação de leads e autoridade visual.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/600x400/?ecommerce" alt="Projeto 2">
        <h3>Loja Online</h3>
        <p>Site de e-commerce integrado com pagamentos, identidade visual e SEO otimizado.</p>
      </div>
    </div>
  </section>  <section id="contato" class="contact">
    <h2 class="section-title">Fale Conosco</h2>
    <p>Quer um site assim? Manda sua mensagem!</p>
    <form action="https://formsubmit.co/seuemail@gmail.com" method="POST">
      <input type="text" name="nome" placeholder="Seu nome" required>
      <input type="email" name="email" placeholder="Seu e-mail" required>
      <textarea name="mensagem" rows="5" placeholder="Escreva sua mensagem aqui..." required></textarea>
      <button type="submit">Enviar</button>
    </form>
  </section>  <footer>
    <p>&copy; 2025 NexusBM — Criado com dedicação por Luiz Martins e Victor Baldez.</p>
  </footer>
</body>
</html>