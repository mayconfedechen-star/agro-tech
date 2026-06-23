<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AgroTech - Ensaios Agrícolas</title>

<style>
body{
    font-family: Arial, sans-serif;
    margin:0;
    background:#f4f4f4;
}

header{
    background:#2e7d32;
    color:white;
    text-align:center;
    padding:20px;
}

nav{
    background:#1b5e20;
    text-align:center;
    padding:10px;
}

nav a{
    color:white;
    text-decoration:none;
    margin:0 15px;
    font-weight:bold;
}

section{
    padding:20px;
}

.card{
    background:white;
    padding:15px;
    margin:15px 0;
    border-radius:10px;
    box-shadow:0 2px 5px rgba(0,0,0,0.1);
}

img{
    max-width:100%;
    border-radius:8px;
}

table{
    width:100%;
    border-collapse:collapse;
    font-family:Arial, sans-serif;
}

th,td{
    border:1px solid #ddd;
    padding:8px;
    text-align:left;
}

th{
    background:#f2f2f2;
}

footer{
    background:#2e7d32;
    color:white;
    text-align:center;
    padding:10px;
    margin-top:20px;
}

/* Login */
#loginBox{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background:#f4f4f4;
    display:flex;
    justify-content:center;
    align-items:center;
    z-index:9999;
}

.login-container{
    background:white;
    padding:30px;
    border-radius:10px;
    box-shadow:0 0 10px rgba(0,0,0,0.2);
    text-align:center;
    width:300px;
}

.login-container input{
    width:90%;
    padding:10px;
    margin:10px 0;
}

.login-container button{
    padding:10px 20px;
    background:#2e7d32;
    color:white;
    border:none;
    border-radius:5px;
    cursor:pointer;
}

#erro{
    color:red;
}
</style>
</head>

<body>

<!-- LOGIN -->
<div id="loginBox">
    <div class="login-container">
        <h2>Identificação</h2>

        <input type="text" id="usuario" placeholder="Usuário">
        <input type="password" id="senha" placeholder="Senha">

        <button onclick="entrar()">Entrar</button>

        <p id="erro"></p>
    <div class="card">
    <h3>Importância</h3>

    <p>
        Esses ensaios ajudam produtores a tomar decisões mais assertivas,
        aumentando a eficiência da produção e reduzindo riscos.
    </p>

    <img src="https://agrotools.com.br/wp-content/uploads/2021/06/agrotools-artigo-agricultura-digital.jpg"
         alt="Agricultura Digital">
</div>


<header>
    <h1>AgroTech</h1>
    <p>Inovação no Campo com Ensaios Agrícolas</p>
</header>

<nav>
    <a href="#inicio">Início</a>
    <a href="#sobre">Sobre</a>
    <a href="#ensaios">Ensaios</a>
    <a href="#contato">Contato</a>
</nav>

<section id="sobre">
    <div class="card">
        <h2>O que é Agro Tech?</h2>
        <p>
            Agro Tech é o uso de tecnologia no agronegócio para aumentar a produtividade,
            reduzir custos e melhorar a qualidade das produções agrícolas.
        </p>

        <img src="https://aegro.com.br/images/blog/geradas/agricultura-digital-ferramentas-tendencias-e-desafios-para-o-produtor-rural.webp"
             alt="Agricultura Digital">
    </div>
</section>

<section id="ensaios">

    <div class="card">
        <h2>Ensaios Agrícolas</h2>

        <p>
            Os ensaios agrícolas são testes realizados no campo para avaliar o desempenho
            de sementes, fertilizantes, defensivos e técnicas de cultivo.
        </p>

        <img src="https://www.produzindocerto.com.br/wp-content/uploads/2022/01/blog-IG-dicionagro-S17-24-01.jpg"
             alt="O Agro é Tech">
    </div>

    <div class="card">
        <h3>Tipos de Ensaios</h3>

        <ul>
            <li>Ensaios de produtividade</li>
            <li>Ensaios de variedades</li>
            <li>Ensaios de fertilização</li>
            <li>Ensaios de controle de pragas</li>
        </ul>
    </div>

        <p>
            Esses ensaios ajudam produtores a tomar decisões mais assertivas,
            aumentando a eficiência da produção e reduzindo riscos.
        </p>

        <img src="https://agrotools.com.br/wp-content/uploads/2021/06/agrotools-artigo-agricultura-digital.jpg"
             alt="Agricultura Digital">
    </div>

</section>

<section id="contato">
    <div class="card">
        <h2>Localização</h2>

        <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d14511.735202110038!2d-52.28882953307229!3d-24.59148074969135!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94eddbf8811d649d%3A0x7b5fc5cca0c1b0cb!2sRoncador%2C%20PR%2C%2087320-000!5e0!3m2!1spt-BR!2sbr!4v1781524035088!5m2!1spt-BR!2sbr"
            width="100%"
            height="400"
            style="border:0;"
            allowfullscreen=""
            loading="lazy">
        </iframe>
    </div>
</section>

<script>
function entrar() {
    const usuario = document.getElementById("usuario").value;
    const senha = document.getElementById("senha").value;

    if (usuario === "admin" && senha === "1234") {
        document.getElementById("loginBox").style.display = "none";
    } else {
        document.getElementById("erro").textContent =
            "Usuário ou senha incorretos!";
    }
}
</script>

</body>
</html>
    


