<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Serralheria Renó - Qualidade e Confiança</title>
  <style>
    /* Reset simples */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #f5f5f5;
      color: #333;
      line-height: 1.6;
    }
    header {
      background: #222;
      color: #fff;
      padding: 20px 10%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 10;
    }
    header h1 {
      font-size: 24px;
      letter-spacing: 2px;
      font-weight: 700;
      cursor: default;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      margin-left: 25px;
      font-weight: 600;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: #e63946;
    }
    .banner {
      background: url('https://images.unsplash.com/photo-1542834369-f10ebf06d3cb?auto=format&fit=crop&w=1400&q=80') no-repeat center center/cover;
      height: 350px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      text-shadow: 2px 2px 8px #000;
      font-size: 2rem;
      font-weight: 700;
      text-align: center;
      padding: 0 20px;
    }
    main {
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
    }
    section {
      margin-bottom: 50px;
    }
    h2 {
      color: #222;
      margin-bottom: 15px;
      border-bottom: 3px solid #e63946;
      display: inline-block;
      padding-bottom: 5px;
    }
    /* Serviços */
    .servicos-lista {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 25px;
    }
    .servico-item {
      background: #fff;
      padding: 20px;
      border-radius: 6px;
      box-shadow: 0 2px 6px rgb(0 0 0 / 0.1);
      transition: transform 0.3s ease;
    }
    .servico-item:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 15px rgb(0 0 0 / 0.15);
    }
    .servico-item img {
      max-width: 100%;
      border-radius: 4px;
      margin-bottom: 12px;
      height: 140px;
      object-fit: cover;
    }
    /* Galeria */
    .galeria-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 15px;
    }
    .galeria-grid img {
      width: 100%;
      height: 140px;
      object-fit: cover;
      border-radius: 6px;
      cursor: pointer;
      transition: transform 0.25s ease;
    }
    .galeria-grid img:hover {
      transform: scale(1.05);
    }
    /* Formulário Orçamento */
    form {
      background: #fff;
      padding: 25px;
      border-radius: 6px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      max-width: 500px;
      margin: auto;
    }
    form label {
      display: block;
      margin-bottom: 8px;
      font-weight: 600;
    }
    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 18px;
      border: 1px solid #ccc;
      border-radius: 4px;
      resize: vertical;
      font-size: 1rem;
      font-family: inherit;
    }
    form button {
      background: #e63946;
      color: #fff;
      border: none;
      padding: 12px 25px;
      font-size: 1.1rem;
      border-radius: 4px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    form button:hover {
      background: #d62828;
    }
    /* Sobre */
    .sobre-texto {
      max-width: 700px;
      margin: auto;
      background: #fff;
      padding: 25px;
      border-radius: 6px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      font-size: 1.1rem;
      line-height: 1.8;
      color: #444;
    }
    /* Contato */
    .contato-info {
      max-width: 700px;
      margin: auto;
      background: #fff;
      padding: 25px;
      border-radius: 6px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      font-size: 1.1rem;
      color: #444;
    }
    .contato-info p {
      margin-bottom: 12px;
    }
    .mapa {
      margin-top: 20px;
      width: 100%;
      height: 300px;
      border-radius: 6px;
      overflow: hidden;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    /* Footer */
    footer {
      background: #222;
      color: #ccc;
      text-align: center;
      padding: 15px 10%;
      font-size: 0.9rem;
    }

    /* Responsividade */
    @media (max-width: 600px) {
      header {
        flex-direction: column;
        text-align: center;
        gap: 10px;
      }
      nav a {
        margin-left: 0;
        margin-right: 15px;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Serralheria Renó</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#servicos">Serviços</a>
      <a href="#galeria">Galeria</a>
      <a href="#orcamento">Orçamento</a>
      <a href="#sobre">Sobre</a>
      <a href="#contato">Contato</a>
    </nav>
  </header>

  <section class="banner" id="home">
    Qualidade e confiança para o seu projeto em serralheria
  </section>

  <main>
    <section id="servicos">
      <h2>Serviços</h2>
      <div class="servicos-lista">
        <div class="servico-item">
          <img src="https://images.unsplash.com/photo-1590080877777-0b15fae04f3e?auto=format&fit=crop&w=600&q=80" alt="Portão de ferro" />
          <h3>Portões de Ferro e Alumínio</h3>
          <p>Fabricação e instalação de portões resistentes e personalizados para sua casa ou empresa.</p>
        </div>
        <div class="servico-item">
          <img src="https://images.unsplash.com/photo-1602524812679-6b5a372773e4?auto=format&fit=crop&w=600&q=80" alt="Grades de proteção" />
          <h3>Grades de Proteção</h3>
          <p>Grades de segurança para portas e janelas, garantindo proteção e beleza ao imóvel.</p>
        </div>
        <div class="servico-item">
          <img src="https://images.unsplash.com/photo-1581093588401-2d6e3a466e88?auto=format&fit=crop&w=600&q=80" alt="Guarda corpo" />
          <h3>Guarda-Corpos e Corrimãos</h3>
          <p>Produção de guarda-corpos resistentes para escadas e sacadas, com acabamento impecável.</p>
        </div>
        <div class="servico-item">
          <img src="https://images.unsplash.com/photo-1566843977961-3c1f44f82de5?auto=format&fit=crop&w=600&q=80" alt="Escora metálica" />
          <h3>Aluguel de Escoras Metálicas e Andaimes</h3>
          <p>Equipamentos para construção e reformas, com segurança e qualidade para seu trabalho.</p>
        </div>
        <div class="servico-item">
          <img src="https://images.unsplash.com/photo-1554224154-22dec7ec8818?auto=format&fit=crop&w=600&q=80" alt="Manutenção" />
          <h3>Manutenção e Reformas</h3>
          <p>Serviços de reparo e manutenção para garantir durabilidade e segurança das estruturas metálicas.</p>
        </div>
      </div>
    </section>

    <section id="galeria">
      <h2>Galeria</h2>
      <div class="galeria-grid">
        <img src="https://images.unsplash.com/photo-1590080877777-0b15fae04f3e?auto=format&fit=crop&w=600&q=80" alt="Portão de ferro" />
        <img src="https://images.unsplash.com/photo-1602524812679-6b5a372773e4?auto=format&fit=crop&w=600&q=80" alt="Grades de proteção" />
        <img src="https://images.unsplash.com/photo-1581093588401-2d6e3a466e88?auto=format&fit=crop&w=600&q=80" alt="Guarda corpo" />
        <img src="https://images.unsplash.com/photo-1566843977961-3c1f44f82de5?auto=format&fit=crop&w=600&q=80" alt="Escora metálica" />
        <img src="https://images.unsplash.com/photo-1554224154-22dec7ec8818?auto=format&fit=crop&w=600&q=80" alt="Manutenção" />
      </div>
    </section>

    <section id="orcamento">
      <h2>Peça seu Orçamento</h2>
      <form id="formOrcamento">
        <label for="nome">Nome completo</label>
        <input type="text" id="nome" name="nome" placeholder="Seu nome" required />

        <label for="telefone">Telefone / WhatsApp</label>
        <input type="tel" id="telefone" name="telefone" placeholder="(xx) xxxxx-xxxx" required />

        <label for="email">E-mail</label>
        <input type="email" id="email" name="email" placeholder="seu@email.com" required />

        <label for="mensagem">Descrição do serviço</label>
        <textarea id="mensagem" name="mensagem" rows="5" placeholder="Explique o que deseja" required></textarea>

        <button type="submit">Enviar Pedido</button>
      </form>
    </section>

    <section id="sobre">
      <h2>Sobre a Serralheria Renó</h2>
      <div class="sobre-texto">
        <p>Com anos de experiência no mercado, a Serralheria Renó é referência em qualidade e confiança para serviços em metalurgia e serralheria. Nosso compromisso é entregar soluções personalizadas, duráveis e com excelente acabamento para cada cliente.</p>
        <p>Atendemos residências, comércios e indústrias, com rapidez e profissionalismo. Nossa equipe é treinada e dedicada para garantir sua satisfação total.</p>
      </div>
    </section>

    <section id="contato">
      <h2>Contato</h2>
      <div class="contato-info">
        <p><strong>Telefone / WhatsApp:</strong> <a href="https://wa.me/5535999397925" target="_blank" rel="noopener noreferrer">(35) 99939-7925</a></p>
        <p><strong>E-mail:</strong> contato@serralheriareno.com.br</p>
        <p><strong>Endereço:</strong> Rua das Flores, 123 - Centro, Sua Cidade - MG</p>

        <div class="mapa">
          <iframe 
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3723.3904919510286!2d-44.19901368492747!3d-20.35675318642521!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xa5a4f8ca0a1d4e3%3A0x7d7f8f874d7ef3f9!2sRua%20das%20Flores%2C%20123%20-%20Centro%2C%20%C3%8Dndios%20-%20MG!5e0!3m2!1spt-BR!2sbr!4v1625234567890!5m2!1spt-BR!2sbr" 
            width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
        </div>
      </div>
    </section>
  </main>

  <footer>
    &copy; 2025 Serralheria Renó | Todos os direitos reservados
  </footer>

  <script>
    // Exemplo simples de validação e envio do formulário - aqui só vai mostrar alerta
    const form = document.getElementById('formOrcamento');
    form.addEventListener('submit', e => {
      e.preventDefault();
      alert('Obrigado pelo seu contato, ' + form.nome.value + '! Em breve entraremos em contato.');
      form.reset();
    });
  </script>
</body>
</html>
