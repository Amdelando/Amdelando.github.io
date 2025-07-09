<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NexusBM | Serviços Digitais</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Inter', sans-serif;
      margin: 0;
      background-color: #f7f8fa;
      color: #111;
    }
    header {
      background-color: #1a1a1a;
      color: white;
      padding: 40px 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2.5rem;
    }
    header p {
      font-size: 1.1rem;
      margin-top: 10px;
    }
    nav {
      background-color: #292929;
      padding: 10px 20px;
      text-align: center;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: 600;
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }
    .section-title {
      font-size: 2rem;
      margin-bottom: 20px;
      text-align: center;
    }
    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }
    .service {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    }
    .contact {
      background: #eaeaea;
      padding: 40px 20px;
      border-radius: 12px;
      text-align: center;
    }
    footer {
      background-color: #1a1a1a;
      color: white;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>NexusBM</h1>
    <p>Conectando ideias para o sucesso digital.</p>
  </header>

  <nav>
    <a href="#sobre">Sobre</a>
    <a href="#servicos">Serviços</a>
    <a href="#portfolio">Portfólio</a>
    <a href="#contato">Contato</a>
  </nav>

  <section id="sobre">
    <h2 class="section-title">Sobre Nós</h2>
    <p>A NexusBM é formada por Luiz Martins e Victor Baldez, especialistas em soluções digitais que geram resultados reais. Ajudamos empresas a crescer com estratégias inteligentes e visuais impactantes.</p>
  </section>

  <section id="servicos">
    <h2 class="section-title">Serviços</h2>
    <div class="services-grid">
      <div class="service">
        <h3>Gestão de Tráfego Pago</h3>
        <p>Campanhas segmentadas no Google e redes sociais para atrair mais clientes.</p>
      </div>
      <div class="service">
        <h3>Criação de Sites</h3>
        <p>Sites modernos, rápidos e responsivos com foco em conversão.</p>
      </div>
      <div class="service">
        <h3>Copywriting</h3>
        <p>Textos persuasivos que geram ação, vendas e conexão com o público.</p>
      </div>
      <div class="service">
        <h3>Design Gráfico</h3>
        <p>Identidade visual, logos, flyers e layouts com estética e estratégia.</p>
      </div>
      <div class="service">
        <h3>Especialista CTO</h3>
        <p>Orientação técnica e suporte para projetos digitais com visão de futuro.</p>
      </div>
      <div class="service">
        <h3>Google Meu Negócio</h3>
        <p>Coloque sua empresa em destaque nos resultados de busca local.</p>
      </div>
    </div>
  </section>

  <section id="portfolio">
    <h2 class="section-title">Portfólio</h2>
    <p>Em breve você poderá conferir aqui nossos projetos recentes de sites, artes gráficas e campanhas digitais.</p>
  </section>

  <section id="contato" class="contact">
    <h2 class="section-title">Fale Conosco</h2>
    <p>Quer transformar o seu negócio? Fale com a gente:</p>
    <p><strong>WhatsApp:</strong> (xx) xxxxx-xxxx<br />
       <strong>E-mail:</strong> contato@nexusbm.com.br<br />
       <strong>Instagram:</strong> @nexusbm.digital</p>
  </section>

  <footer>
    <p>&copy; 2025 NexusBM — Todos os direitos reservados.</p>
  </footer>
</body>
</html>