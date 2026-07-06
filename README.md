<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Terra Forte — Agro Sustentabilidade</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <div class="container">
      <h1 class="brand">Terra Forte</h1>
      <nav>
        <a href="#sobre">Sobre</a>
        <a href="#praticas">Práticas</a>
        <a href="#projetos">Projetos</a>
        <a href="#galeria">Galeria</a>
        <a href="#contato">Contato</a>
      </nav>
    </div>
  </header>

  <main>
    <section id="hero" class="hero">
      <div class="container hero-inner">
        <div class="hero-text">
          <h2>Agro que preserva a natureza e garante o futuro</h2>
          <p>Inovação, cuidado com o solo e comunidades fortes — conheça o movimento Terra Forte.</p>
          <div class="hero-actions">
            <a class="btn" href="#projetos">Nossos projetos</a>
            <button id="openVideo" class="btn btn-outline">Assista</button>
          </div>
        </div>
        <div class="hero-media">
          <img class="media-img" src="images/hero.svg" alt="Ilustração agro sustentável Terra Forte">
        </div>
      </div>
    </section>

    <section id="sobre" class="container">
      <h3>Sobre</h3>
      <p>Terra Forte é um projeto colaborativo focado em práticas agroecológicas, recuperação de solos e economia local. Trabalhamos com pequenos produtores para implantar técnicas de manejo que aumentem a resiliência climática e a renda familiar.</p>
    </section>

    <section id="praticas" class="container cards">
      <h3>Práticas sustentáveis</h3>
      <div class="card">
        <img data-src="images/agro1.svg" alt="Adubação verde" class="thumb lazy">
        <h4>Adubação verde</h4>
        <p>Uso de plantas de cobertura para aumentar matéria orgânica e proteger o solo.</p>
        <button class="btn btn-small openModal" data-title="Adubação verde" data-text="Plantas de cobertura, como crotalária e mucuna, protegem o solo e suprimentos nutricionais naturais.">Saiba mais</button>
      </div>

      <div class="card">
        <img data-src="images/agro2.svg" alt="Agrofloresta" class="thumb lazy">
        <h4>Agrofloresta</h4>
        <p>Sistemas integrados de árvores, culturas e criação que aumentam biodiversidade.</p>
        <button class="btn btn-small openModal" data-title="Agrofloresta" data-text="Combinação de árvores com cultivos e criação promove múltiplos produtos e estabilidade ecológica.">Saiba mais</button>
      </div>

      <div class="card">
        <img data-src="images/agro3.svg" alt="Manejo de água" class="thumb lazy">
        <h4>Uso eficiente da água</h4>
        <p>Técnicas de irrigação e armazenamento para reduzir desperdício e conservar recursos.</p>
        <button class="btn btn-small openModal" data-title="Uso eficiente da água" data-text="Técnicas como gotejamento e cisternas comunitárias ajudam a otimizar o uso hídrico.">Saiba mais</button>
      </div>
    </section>

    <section id="projetos" class="container">
      <h3>Projetos</h3>
      <p>Recuperação de áreas degradadas, hortas escolares, capacitação técnica e feiras locais de comércio justo.</p>
      <ul>
        <li>Projeto Solo Vivo — recuperação com adubação verde e compostagem</li>
        <li>Agrofloresta Comunitária — implantação em pequenas propriedades</li>
        <li>Hortas Escolares — educação alimentar e prática</li>
      </ul>
    </section>

    <section id="galeria" class="container">
      <h3>Galeria</h3>
      <div class="carousel" aria-roledescription="carousel">
        <button class="carousel-btn prev" aria-label="Anterior">◀</button>
        <div class="slides">
          <img data-src="images/agro1.svg" alt="Campo com cultivo" class="slide lazy">
          <img data-src="images/agro2.svg" alt="Agrofloresta" class="slide lazy">
          <img data-src="images/agro3.svg" alt="Uso eficiente de água" class="slide lazy">
        </div>
        <button class="carousel-btn next" aria-label="Próximo">▶</button>
      </div>
    </section>

    <section id="contato" class="container">
      <h3>Contato</h3>
      <form id="contactForm" class="form" novalidate>
        <label>Nome
          <input type="text" name="nome" id="nome" required>
        </label>
        <label>Email
          <input type="email" name="email" id="email" required>
        </label>
        <label>Mensagem
          <textarea name="mensagem" id="mensagem" rows="4" required></textarea>
        </label>
        <button type="submit" class="btn">Enviar</button>
        <p id="formStatus" class="muted" aria-live="polite"></p>
      </form>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>&copy; 2026 Terra Forte — Todos os direitos reservados.</p>
    </div>
  </footer>

  <!-- Modal -->
  <div id="modal" class="modal" role="dialog" aria-modal="true" aria-hidden="true">
    <div class="modal-content">
      <button id="closeModal" class="modal-close" aria-label="Fechar">×</button>
      <h4 id="modalTitle"></h4>
      <p id="modalText"></p>
    </div>
  </div>

  <script src="scripts.js"></script>
</body>
</html>
