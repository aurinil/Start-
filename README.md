# Start-
Peças automotivas 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Start Ar Condicionado</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: Arial, sans-serif;
}

body{
    background:#f5f7fa;
    color:#333;
}

header{
    background:#0b4f8a;
    color:white;
    padding:15px 5%;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    display:flex;
    align-items:center;
    gap:10px;
}

.logo img{
    height:60px;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:20px;
    font-weight:bold;
}

.hero{
    background:linear-gradient(rgba(11,79,138,0.8), rgba(11,79,138,0.8)),
    url('https://images.unsplash.com/photo-1581092580497-e0d23cbdf1dc?w=1200');
    background-size:cover;
    background-position:center;
    color:white;
    text-align:center;
    padding:100px 20px;
}

.hero h1{
    font-size:3rem;
    margin-bottom:15px;
}

.hero p{
    font-size:1.2rem;
    margin-bottom:25px;
}

.btn{
    background:#25D366;
    color:white;
    padding:15px 30px;
    border-radius:8px;
    text-decoration:none;
    font-weight:bold;
}

section{
    padding:60px 5%;
}

.titulo{
    text-align:center;
    margin-bottom:40px;
    color:#0b4f8a;
}

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.card{
    background:white;
    padding:25px;
    border-radius:10px;
    box-shadow:0 3px 10px rgba(0,0,0,0.1);
}

.card h3{
    margin-bottom:10px;
    color:#0b4f8a;
}

.formulario{
    background:white;
    padding:30px;
    border-radius:10px;
    max-width:700px;
    margin:auto;
}

input, textarea{
    width:100%;
    padding:12px;
    margin:10px 0;
    border:1px solid #ccc;
    border-radius:5px;
}

button{
    background:#0b4f8a;
    color:white;
    border:none;
    padding:15px;
    width:100%;
    border-radius:5px;
    cursor:pointer;
}

footer{
    background:#0b4f8a;
    color:white;
    text-align:center;
    padding:20px;
}

@media(max-width:768px){
.hero h1{
    font-size:2rem;
}
nav{
    display:none;
}
}
</style>

</head>
<body>

<header>
    <div class="logo">
        <img src="logo.png" alt="Start Ar Condicionado">
        <h2>Start Ar Condicionado</h2>
    </div>

    <nav>
        <a href="#servicos">Serviços</a>
        <a href="#vendas">Vendas</a>
        <a href="#contato">Contato</a>
    </nav>
</header>

<section class="hero">
    <h1>Climatização com Qualidade</h1>
    <p>Venda, instalação e manutenção de ar-condicionado residencial e comercial.</p>

    <a class="btn"
    href="https://wa.me/5515999999999"
    target="_blank">
    Solicitar Orçamento
    </a>
</section>

<section id="servicos">
    <h2 class="titulo">Nossos Serviços</h2>

    <div class="cards">

        <div class="card">
            <h3>Venda</h3>
            <p>Equipamentos das melhores marcas do mercado.</p>
        </div>

        <div class="card">
            <h3>Instalação</h3>
            <p>Equipe qualificada e atendimento rápido.</p>
        </div>

        <div class="card">
            <h3>Manutenção</h3>
            <p>Preventiva e corretiva para todos os modelos.</p>
        </div>

        <div class="card">
            <h3>Higienização</h3>
            <p>Limpeza completa para maior eficiência e saúde.</p>
        </div>

    </div>
</section>

<section id="vendas">
    <h2 class="titulo">Solicitação de Compra</h2>

    <div class="formulario">
        <form onsubmit="enviarWhatsApp(event)">
            <input type="text" id="nome" placeholder="Nome" required>

            <input type="tel" id="telefone" placeholder="Telefone" required>

            <input type="text" id="produto" placeholder="Modelo ou Produto desejado" required>

            <textarea id="mensagem" rows="5" placeholder="Detalhes do pedido"></textarea>

            <button type="submit">Enviar Pedido</button>
        </form>
    </div>
</section>

<section id="contato">
    <h2 class="titulo">Contato</h2>

    <div class="formulario">
        <p><strong>Telefone:</strong> (15) 99999-9999</p>
        <br>
        <p><strong>E-mail:</strong> contato@startarcondicionado.com.br</p>
        <br>
        <p><strong>Atendimento:</strong> Segunda a Sábado</p>
    </div>
</section>

<footer>
    <p>© 2026 Start Ar Condicionado - Todos os direitos reservados.</p>
</footer>

<script>
function enviarWhatsApp(event){
event.preventDefault();

let nome = document.getElementById('nome').value;
let telefone = document.getElementById('telefone').value;
let produto = document.getElementById('produto').value;
let mensagem = document.getElementById('mensagem').value;

let texto =
`*NOVO PEDIDO*%0A
Nome: ${nome}%0A
Telefone: ${telefone}%0A
Produto: ${produto}%0A
Mensagem: ${mensagem}`;

window.open(
'https://wa.me/551533732418?text=' + texto,
'_blank'
);
}
</script>

</body>
</html>
.
