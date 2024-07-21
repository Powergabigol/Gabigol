<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página com Fundo Preto e Imagem</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-color: black;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            height: 100vh;
            overflow: hidden;
            text-align: center;
            position: relative;
            color: white;
            font-family: Arial, sans-serif; /* Fonte padrão */
        }
        .background-image {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('https://imguh.com/images/2024/07/20/e6b1e30637881ae3d19f546dd87aebed12077932b020cb4b.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            background-position: center;
            opacity: 0.3; /* Ajuste a opacidade conforme necessário */
            z-index: -1;
        }
        .container {
            position: relative;
            z-index: 1;
        }
        .container img {
            width: 300px; /* Ajuste o tamanho conforme necessário */
            height: auto;
        }
        .container p {
            margin-top: 10px; /* Ajuste a margem conforme necessário */
            font-size: 18px;
            font-weight: bold;
            font-family: "Helvetica", "Arial", sans-serif; /* Fonte especificada */
        }
        .description {
            margin-top: 20px;
            font-size: 18px;
            font-weight: bold;
            font-family: "Copperplate Gothic", "Copperplate", "Garamond", serif; /* Fonte especificada */
            line-height: 1.6; /* Ajusta o espaçamento entre linhas para melhor legibilidade */
            max-width: 800px; /* Limita a largura do texto para melhor leitura */
            margin-left: auto;
            margin-right: auto;
            white-space: pre-wrap; /* Mantém as quebras de linha */
            overflow: hidden;
            border-right: 3px solid white; /* Efeito de cursor */
            animation: typing 5s steps(100, end), blink-caret 0.75s step-end infinite;
        }
        .button-container {
            margin-top: 20px;
        }
        .button-container a {
            text-decoration: none;
            color: white;
            background-color: gray;
            padding: 10px 20px;
            font-size: 18px;
            border-radius: 5px;
        }

        /* Efeitos de digitação */
        @keyframes typing {
            from { width: 0; }
            to { width: 100%; }
        }

        @keyframes blink-caret {
            from, to { border-color: transparent; }
            50% { border-color: white; }
        }
    </style>
</head>
<body>
    <div class="background-image"></div>
    <div class="container">
        <img src="https://imguh.com/images/2024/07/20/abbd5b9abfee71a9eed081c2dc8ca5429e9bd39b2de2e9e4.png" alt="Imagem Central">
        <p>Gabriel Barbosa Almeida</p>
        <p class="description" id="typing-text">
            Gabriel Barbosa (mais conhecido como Gabigol) é o melhor jogador brasileiro em atividade, com vários recordes e feitos, como: ser o maior artilheiro da história da Libertadores, o maior artilheiro do Flamengo no século 21, ser o terceiro artilheiro da história da Copa do Brasil, entre outros. Gabigol é o principal nome quando o assunto é ser decisivo em grandes campeonatos na América do Sul, com atualmente 4 gols em 3 finais de Libertadores. Isso é uma das várias façanhas feitas por esse jogador. INCRÍVEL!
        </p>
        <div class="button-container">
            <a href="https://youtu.be/el1YRbnFe20?si=yWMgtzwx41O8Jwzm" target="_blank">Veja</a>
        </div>
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const text = document.getElementById("typing-text");
            text.style.animation = "typing 5s steps(100, end), blink-caret 0.75s step-end infinite";
        });
    </script>
</body>
</html>
