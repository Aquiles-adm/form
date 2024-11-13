<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Cadastro</title>
</head>
<body>
    <!--Código Principal-->
    <header>
        <section>
            <img src="cabeca-logo.png" alt="Logo com imagem de um rosto">
            <img src="aura-logo.png" alt="Logo com o texto Aura">
            <ul>
                <li>Allan Dellon</li>
                <li>Lucas Gomes</li>
                <li>Luiz Henrique</li>
                <li>Aquiles De Melo</li>
                <li>Vinicius Barbosa</li>
            </ul>
            <nav>
                <ul>
                    <li><a href="main.html">Home</a></li>
                    <li><a href="galeria.html">Galeria</a></li>
                    <li><a href="cadastro.html">Cadastro</a></li>
                </ul>
            </nav>
        </section>
    </header>
    <!--Código Principal-->
    <main>

        <article>
            <h2>Cadastre-se para saber mais!</h2>
            <form>
                <label for="nome">Nome:</label>
                <input type="text" id="nome" name="nome">

                <label for="email">E-mail:</label>
                <input type="email" id="email" name="email">   


                <label for="mensagem">Sua opinião sobre o site:</label>
                <textarea id="mensagem" name="mensagem"></textarea>

                <button type="submit">Enviar</button>
            </form>
        </article>

        <style>
            h2 {
                text-align: center;
            }
            </style>


    </main>
    <!--Código Do Rodapé-->
    <footer>
        <section>
            <p>Developed by</p>
            <img src="cabeca-logo.png" alt="">
            <img src="aura-logo.png" alt="">
        </section>
    </footer>
</body>
</html>


CSS

 @import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap');
 

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: "Montserrat", sans-serif; /* Fonte*/
}

html {
    scroll-behavior: smooth;
}
body {
    background-image: url(aura-logo.png);
    background-size: 10%;
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-position: center;
}

header {
   position: fixed;
    height: 100px;
    width: 1300px;
    border: 3px solid black;
    margin-left: 10px; /*Margem pra não encostar na borda*/
    display: flex;
    border-radius: 80px;
    margin-top: 20px; /*Margem pra não encostar em cima*/
    z-index: 10;
    background-color: white;
}

header section {
    display: flex;
    text-align: center;
    width: 100%;
}

/*Configurações da imagem-logo*/
header img {
    width: 90px;
    height: 92px;
    border-radius: 100px;
    margin: 1px;
    display: inline;
}

header ul {
    display: flex;
    list-style: none;
    gap: 9.5px;
}
/*Configurações dos nomes dos participantes*/
header li {
    color: rgb(0, 0, 0);
    margin-top: 35px;
    margin-left: 14px;
    font-size: 14px;
}
/*Destaque quando passar o mouse*/
header li:hover {
    font-size: 17px;
    transition: font-size 0.3s ease;
    color: rgb(255, 0, 0);
}
/*Menu "Home", "Galeria"e"Cadastro"*/

header nav {
    margin-left: 10px;
}

nav a {
    text-decoration: none;
    color: rgb(0, 0, 0);
    margin-left: 80px;
}

main {
    padding-top: 120px;
    margin-bottom: 50px;
    gap: 500px;

/* Estilizando o formulário */
form {
    max-width: 400px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: #f9f9f9;
  }
  
  /* Estilizando os labels e inputs */
  label {
    display: block;
    margin-bottom: 10px;
  }
  
  input,
  textarea {
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    box-sizing: border-box;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  
  /* Estilizando o botão */
  button[type="submit"] {
    background-color: #4CAF50;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }

}


.integrantes  {
    position: relative; 
    margin-right: 1000px;
}

.integrantes img {
    margin-top: 10px;
    margin-left: 30px;
    width: 220px;
    border-radius: 30px;
    border: 3px solid rgb(0, 0, 0);
    transition: 0.5s ease;
    margin-bottom: 20px;
}

.integrantes:hover img {
    width: 300px;
    transition: 0.5s ease;
}

.integrantes .descricao {
    position: absolute;
    bottom: 0;
    left: 0;
    height: 300px;
    width: 500px;
    font-size: 20px;
    transform: translateX(0);
    transition: transform 0.8s ease;
    padding: 1px;
    margin-left: 20px;
    visibility: hidden;
    color: red;
}

.integrantes:hover .descricao {
    visibility: visible;
    transform: translateX(65%);
}

footer {
    background-color: rgb(255, 255, 255);
}

footer {
    text-align: center;
}

footer img {
    display: inline;
    border-radius: 100px;
    width: 100px;
}























