<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tu é?</title>
<style>
    body {
        margin: 0;
        padding: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        height: 100vh;
        background-color: black; /* Alterando para fundo preto */
        color: white; /* Alterando a cor do texto para branco */
    }

    .container {
        position: relative;
        text-align: center;
        margin-bottom: 20px;
    }

    button {
        width: 150px;
        height: 50px;
        font-size: 16px;
        border: 2px solid white; /* Mantendo a borda branca */
        cursor: pointer;
    }

    #sim {
        background-color: #99ff99; /* Cor de fundo verde claro */
        position: absolute;
        left: calc(50% - 175px);
    }

    #nao {
        background-color: #ff9999; /* Cor de fundo vermelho claro */
        position: absolute;
        right: calc(50% - 175px);
    }

    #pergunta {
        position: relative;
        top: -100px; /* Ajuste para posicionar o texto mais acima */
        font-size: 48px; /* Ajuste para aumentar o tamanho do texto */
    }
</style>
</head>
<body>

<div class="container">
    <p id="pergunta">Tu é?</p>
</div>

<button id="sim" onclick="redirecionar()">Sim</button>
<button id="nao" onmouseover="moverBotaoNao()">Não</button>

<script>
    function moverBotaoNao() {
        var naoButton = document.getElementById("nao");
        var screenWidth = window.innerWidth;
        var screenHeight = window.innerHeight;
        var newLeft = Math.random() * (screenWidth - naoButton.offsetWidth);
        var newTop = Math.random() * (screenHeight - naoButton.offsetHeight);
        naoButton.style.left = newLeft + "px";
        naoButton.style.top = newTop + "px";
    }

    function redirecionar() {
        window.location.href = "https://www.youtube.com/watch?v=tTs0d88OZR8";
    }
</script>

</body>
</html>
# tu_e
