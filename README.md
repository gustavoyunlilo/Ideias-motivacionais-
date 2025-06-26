# Ideias-motivacionais-
Actualização sobre o mundo actual
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>EmpreendeMente</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet" />
  <style>
    :root {
      --primary: #4a7cff;
      --secondary: #ffca3a;
      --dark: #222;
      --light: #f5f5f5;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: "Poppins", sans-serif;
    }

    body {
      background: var(--light);
      color: var(--dark);
      line-height: 1.6;
    }

    /* Header & Navigation */
    header {
      background: var(--primary);
      color: #fff;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    nav ul {
      display: flex;
      gap: 1rem;
      list-style: none;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 600;
    }

    /* Hero */
    .hero {
      padding: 4rem 2rem;
      text-align: center;
      background: #fff;
    }

    .hero h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }

    /* Sections */
    .section {
      padding: 3rem 2rem;
      background: #fff;
      margin: 1rem 0;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.05);
    }

    .section h2 {
      color: var(--primary);
      margin-bottom: 1rem;
    }

    /* Ideas grid */
    .ideas-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1rem;
    }

    .idea {
      padding: 1rem;
      border: 1px solid #ddd;
      border-radius: 8px;
      background: var(--light);
    }

    /* Blog list */
    .blog-list article {
      margin-bottom: 1.5rem;
    }

    /* Email card */
    .email-card {
      max-width: 500px;
      margin: 0 auto;
      padding: 1rem;
      border-radius: 8px;
      background: var(--light);
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }

    form input,
    form textarea {
      width: 100%;
      padding: 0.75rem;
      margin-top: 0.5rem;
      border-radius: 4px;
      border: 1px solid #ccc;
    }

    button {
      margin-top: 1rem;
      padding: 0.75rem 1.5rem;
      border: none;
      border-radius: 4px;
      background: var(--primary);
      color: #fff;
      font-weight: 600;
      cursor: pointer;
    }

    /* Footer */
    footer {
      padding: 2rem;
      text-align: center;
      font-size: 0.875rem;
      color: #555;
    }

    /* Mobile nav toggle */
    #menu-toggle {
      display: none;
      cursor: pointer;
      font-size: 1.5rem;
    }

    @media (max-width: 640px) {
      nav ul {
        position: absolute;
        top: 60px;
        left: 0;
        width: 100%;
        flex-direction: column;
        background: var(--primary);
        display: none;
      }

      nav ul.show {
        display: flex;
      }

      #menu-toggle {
        display: block;
      }
    }
  </style>
  <script>
    function toggleMenu() {
      document.querySelector("nav ul").classList.toggle("show");
    }
  </script>
</head>
<body>
  <header>
    <div style="font-size: 1.25rem; font-weight: 600">EmpreendeMente</div>
    <div id="menu-toggle" onclick="toggleMenu()">☰</div>
    <nav>
      <ul>
        <li><a href="#home">Início</a></li>
        <li><a href="#ideias">Ideias</a></li>
        <li><a href="#psicologia">Psicologia</a></li>
        <li><a href="#blog">Blog</a></li>
        <li><a href="#contato">Contato</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero -->
  <section id="home" class="hero">
    <h1>Bem-vindo ao EmpreendeMente</h1>
    <p>
      Ideias de negócio, psicologia aplicada e um espaço para compartilhar e
      crescer juntos.
    </p>
  </section>

  <!-- Ideias de Empreendimento -->
  <section id="ideias" class="section">
    <h2>Ideias de Empreendimento</h2>
    <div class="ideas-grid">
      <div class="idea">
        <h3>Loja Virtual de Produtos Artesanais</h3>
        <p>
          Comece vendendo através de marketplaces enquanto constrói sua marca...
        </p>
      </div>
      <div class="idea">
        <h3>Consultoria Online</h3>
        <p>
          Ofereça sua expertise em uma área específica usando videoconferências...
        </p>
      </div>
      <!-- Adicione mais ideias conforme desejar -->
    </div>
  </section>

  <!-- Psicologia & Dicas -->
  <section id="psicologia" class="section">
    <h2>Psicologia & Dicas</h2>
    <p>Conteúdos para fortalecer sua mentalidade empreendedora.</p>
    <ul>
      <li>Mantenha um diário de gratidão para reduzir ansiedade.</li>
      <li>Use a técnica Pomodoro para foco e produtividade.</li>
      <li>Defina metas SMART.</li>
    </ul>
  </section>

  <!-- Blog -->
  <section id="blog" class="section">
    <h2>Blog</h2>
    <div class="blog-list">
      <article>
        <h3>Como validar sua ideia de negócio em 7 dias</h3>
        <p>Publicado em 26 de junho de 2025</p>
      </article>
      <!-- Adicione novos artigos com facilidade -->
    </div>
  </section>

  <!-- Contato / Interação -->
  <section id="contato" class="section">
    <h2>Interaja Conosco</h2>
    <div class="email-card">
      <p>
        Envie suas dúvidas, ideias ou peça conselhos diretamente no nosso
        e-mail.
      </p>
      <form action="https://formspree.io/f/SEU_ENDPOINT" method="POST">
        <!-- Altere SEU_ENDPOINT pelo ID gerado no Formspree -->
        <label>Seu Nome</label>
        <input type="text" name="name" required />
        <label>Seu E-mail</label>
        <input type="email" name="email" required />
        <label>Mensagem</label>
        <textarea name="message" rows="4" required></textarea>
        <button type="submit">Enviar</button>
      </form>
    </div>
  </section>

  <footer>
    © 2025 EmpreendeMente. Todos os direitos reservados.
  </footer>
</body>
</html>
