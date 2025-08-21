* {
    margin: 0;
    padding: 0;
}

body {
    font-family: Verdana, sans-serif;
    background-color: rgb(95, 92, 86);
    padding: 20px;
    text-align: center;
}

header {
    background-color: rgb(241, 234, 27);
    color: #000000;
    padding: 5px;
    text-align: center;
}

main {
    display: flex;
    background-color: rgb(71, 55, 43);
    padding: 20px;
    justify-content: center;
    
}

form {
    background-color: rgb(147, 141, 141);
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 6px rgba(rgb(0, 0, 0));
    width: 400px;

}

form label {
    font-weight: bold;
    margin-bottom: 5px;
    display: block;
    
}

form input {
    width: 100%;
    padding: 5px;
    margin-bottom: 15px;
    border: 1px solid #ccc;

}

form input:focus {
    border-color: rgb(255, 200, 0);
    outline: none;
}

input {
    width: 95%;
    padding: 5px;
    margin: 8px 0;
    border-radius: 5px;
    border: 1px solid #000000;
    
    

}

button {
    width: 25%;
    padding: 5px;
    background-color: rgb(0, 0, 0);
    border: none;
    color: white;
    border-radius: 10px;
    font-size: 16px;
    cursor: pointer;

}

button:hover {
    background-color: rgb(89, 79, 79);
}

footer {
    width: 100%;
    padding: 20px;
    font-size: small;
    padding: 10px;
    text-align: right;
    text-decoration-line: underline;
    

}

#mensagem{
    margin-top: 20px;
    font-size: 18px;
    font-weight: bold;
    color: blue;
    text-align: center;
}






<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apenas resenha</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1 id="titulo">Cadastro de usuários</h1>

    </header>
    
        <main>
            <section>
                <form id="CadastroForm">
                    
                
                                <label for="nome">Nome: </label>
                                <input type="text" name=""
                                id="nome"
                                placeholder="Digite seu nome aqui:">
                                <label for ="email">E-mail:</label>
                                <input type="email" name="" id="email" placeholder="Digite seu email aqui:">
                                <label for="senha">Senha:</label>
                                <input type="password" name="" id="senha" placeholder="Digite sua senha aqui:">
                                
                
                
                                <button type="submit">ENVIAR</button>
                                <p id="mensagem"></p>
                
                
                
                </form>
            </section>
        </main>

    <footer>
        <p>&copy;Criado por pedro</p>
    </footer>
    <script>
        const form = document.getElementById( 'cadastroForm')
        form.addEventListener('submit', function(event) {
            event.preventDefault();
            const nome = document.getElementById('nome').value;
            document.getElementById('mensagem').textContent =
            "Bem-vindo, " + nome + "! Seu cadastro foi realizado."
        });


    </script>
</body>
</html> 
