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




##css##
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Arial', sans-serif;
}

body {
    background-color: #f4f4f4;
    color: #333;
    background-image: url('imagens/praia\ de\ maceio.png');
     background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: fixed;
}

/* Header */
header {
    background-color: #fff;
    padding: 20px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);

}

.logo {
    font-size: 24px;
    font-weight: bold;
    color: #0077b6;
}
nav ul { list-style: none; }
nav ul li { display: inline; margin-left: 20px; }
nav ul li a { text-decoration: none; color: #333; font-weight: bold; }

.btn-cta {
    background-color: #ff9f1c;
    padding: 10px 20px;
    border-radius: 5px;
    color: rgba(255, 255, 255, 0.785);
}

/* Hero Section */
.hero {
    background-image: linear-gradient(rgba(0,0,0,0.5), rgba(0, 0, 0, 0.5)), url('style.css');
    background-size: cover;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: rgba(255, 255, 255, 0.841);
    padding-top: 80px; /* Espaço pro header fixo */
}
.hero h1 { font-size: 48px; margin-bottom: 20px; }
.hero p { font-size: 20px; margin-bottom: 30px; }

.btn-cta-large {
    background-color: #ff9f1c;
    padding: 15px 30px;
    text-decoration: none;
    color: white;
    font-size: 18px;
    border-radius: 5px;
    font-weight: bold;
}
/* Destinos/Cards */
.card {
    background: #f9f9f97b;
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0 2px 3px rgba(0,0,0,0.1);
}

.destinos { 
    padding: 50px 20px; 
    text-align: center; 
}

/* Configuração da Grid para alinhar os cards lado a lado */
.grid-pacotes {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
  padding: 20px;
  max-width: 1200px;
  margin: 0 auto;
  font-family: Arial, sans-serif;
}

/* Estilização individual de cada Card */
.card {
  background-color: #ffffff;
  border-radius: 12px;
  overflow: hidden; /* Garante que a imagem siga o arredondamento do card */
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  display: flex;
  flex-direction: column;
  padding-bottom: 20px;
}

/* Efeito de levante ao passar o mouse no card */
.card:hover {
  transform: translateY(-6px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
}

/* Configuração das imagens dos cards */
.card img {
  width: 100%;
  height: 200px;
  object-fit: cover; /* Recorta a imagem proporcionalmente sem distorcer */
}

/* Textos internos do card */
.card h3 {
  margin: 16px 16px 8px 16px;
  font-size: 20px;
  color: #333;
}

.card p {
  margin: 0 16px 20px 16px;
  color: #666;
  font-size: 14px;
  line-height: 1.5;
  flex-grow: 1; /* Empurra o botão sempre para o final do card */
}

/* Botão "Saber Mais" */
.btn-card {
  display: inline-block;
  margin: 0 16px;
  padding: 10px;
  background-color: #007BFF;
  color: white;
  text-align: center;
  text-decoration: none;
  font-weight: bold;
  border-radius: 6px;
  transition: background-color 0.2s ease;
}

.btn-card:hover {
  background-color: #0056b3;
}

/* Estilização do texto descritivo (Article) */
.descricao-cidade {
  max-width: 800px;
  margin: 40px auto;
  padding: 0 20px;
  font-family: Arial, sans-serif;
  color: #e6ecf5e9;
  line-height: 1.6;
}

.descricao-cidade h2 {
  color: #333;
  border-bottom: 2px solid #1d19e8;
  padding-bottom: 8px;
}


/* Centraliza e limita a largura do formulário na tela */
form {
  max-width: 400px;
  margin: 40px auto;
  padding: 20px;
  background-color: #f9f9f97b;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  font-family: Arial, sans-serif;
}
.form h2{
 font-weight: bold;
  color: #6397d5;
 text-align: center;
}
/* Organiza os blocos de cada campo com espaçamento inferior */
form div {
  margin-bottom: 16px;
}

/* Estiliza os rótulos de texto */
label {
  display: block;
  margin-bottom: 6px;
  font-weight: bold;
  color: #333333;
}

/* Padroniza as caixas de entrada de texto e e-mail e a área de mensagem */
input[type="text"],
input[type="email"],
textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc0c0;
  border-radius: 4px;
  box-sizing: border-box; /* Garante que o padding não mude o tamanho final */
  font-size: 14px;
}

/* Altera a cor da borda quando o usuário clica no campo */
input:focus,
textarea:focus {
  border-color: #007BFF;
  outline: none; /* Remove a borda padrão do navegador */
}

/* Estiliza o botão de envio */
button[type="submit"] {
  width: 100%;
  padding: 12px;
  background-color: #007BFF;
  color: rgb(144, 137, 137);
  border: none;
  border-radius: 4px;
  font-size: 16px;
  font-weight: bold;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

/* Aplica efeito visual ao passar o mouse sobre o botão */
button[type="submit"]:hover {
  background-color: #b35f00;
}
