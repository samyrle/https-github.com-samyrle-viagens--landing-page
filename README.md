# https-github.com-samyrle-viagens--landing-page
projeto do curso dev start programaçao web - landinpage - agencia de viagens 
# ola me chamo samyrle estudante e iniciante na area de programaçao web 
treinando projetos em front end .


# codigo html 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Agência  Destinos Incríveis</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <div class="logo">Destinos Praias</div>
        <nav>
            <ul>
                <li><a href="#destinos">Minha Viagem</a></li>
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#contato" class="btn-cta">Nos Encontre </a></li>
            </ul>
        </nav>
    </header>
<main>
        <!-- Seção Hero (A primeira dobra) -->
    <section class="hero">
         <div class="hero-content">
            <h1>Descubra o mundo com conforto e exclusividade.</h1>
            <p>Pacotes personalizados para as melhores praias.</p>
            <a href="#contato" class="btn-cta-large">Explore Destinos</a>
        </div>
    </section>

    <!-- Destinos (Grid de Pacotes) -->
    <section id="destinos" class="destinos">
        <h2>Destinos Mais Procurados</h2>
       <div class="grid-pacotes">
    <!-- Card 1 (Camocim) -->
    <div class="card">
        <img src="imagens/praia-barreiras-min.jpg" alt="Praia paradisíaca">
        <h3>Camocim</h3>
        <p>7 dias e hotelaria com tudo incluso.</p>
        <a href="#" class="btn-card">Saber Mais</a>
    </div>

    <!-- Card 2 (Barra dos Remédios) -->
    <div class="card">
        <img src="imagens/praia dos remedios.jpg" alt="praia">
        <h3>Barra dos Remédios</h3>
        <p>Encontro do rio com o mar e dunas.</p>
        <a href="#" class="btn-card">Saber Mais</a>
    </div>

    <!-- Card 3 (Praia do Maceió) -->
    <div class="card">
        <img src="imagens/praia de maceio.png" alt="Praia">
        <h3>Praia do Maceió</h3>
        <p>Tranquilidade e pôr do sol perfeito.</p>
        <a href="#" class="btn-card">Saber Mais</a>
    </div>
</div>
<section id="sobre" class="sobre"></section>
<!-- Artigo de descrição posicionado fora da grid de cards -->
<article class="descricao-cidade">
    <h2>Conheça Camocim</h2>
    <p>Camocim é um município brasileiro no litoral noroeste do estado do Ceará, fundado em 1879 e situado no Litoral do Sol Poente, conhecido por suas praias, dunas e foz do Rio Coreaú.</p>
    <p><strong>Praia da Tatajuba:</strong> Famosa pelas lagoas de águas mornas, dunas móveis e a atração da vila soterrada, sendo excelente para passeios de buggy e kitesurf.</p>
    <p><strong>Praia de Barra dos Remédios:</strong> Considerada uma das mais bonitas, com um encontro espetacular do rio com o mar e dunas imensas, ideal para isolamento e contato com a natureza.</p>
    <p><strong>Praia do Maceió:</strong> Possui águas tranquilas e boas opções de barracas, sendo o local perfeito para ver o pôr do sol.</p>
</article>

                 
            <!-- Adicionar mais cards aqui -->
        </div>
    </section>
    <form action="/enviar-dados" method="POST">
  <h2> Nos enconte </h2>
   <div>
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome" placeholder="Digite seu nome completo" required>
  </div>

  <div>
    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email" placeholder="seu-email@exemplo.com" required>
  </div>

  <div>
    <label for="mensagem">Mensagem:</label>
    <textarea id="mensagem" name="mensagem" rows="4" placeholder="Escreva sua mensagem aqui..."></textarea>
  </div>

  <div>
    <button type="submit">Enviar Formulário</button>
  </div>

</form>

</main>
    <!-- Rodapé (Contato) -->
    <footer id="contato">
        <p>&copy; 2026 Destinos incriveis- Agência de Viagens.</p>
         </footer>

</body>
</html>
