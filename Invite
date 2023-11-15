<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            background-color: #1f1f1f; /* Preto: #1f1f1f */
            color: #ffffff;
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        #invite-container,
        #guild-info-container,
        #journal-container {
            position: relative;
            border-radius: 15px;
            padding: 20px;
            width: 70%;
            max-width: 600px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            overflow: hidden;
            background: linear-gradient(to bottom, #00274e, #0077cc); /* Azul escuro: #00274e, Azul claro: #0077cc */
        }

        .gradient-border {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            pointer-events: none;
            background: linear-gradient(to right, transparent, #ffffff, transparent);
            content: '';
            z-index: -1;
            animation: gradient-animation 2s linear infinite;
        }

        @keyframes gradient-animation {
            0% {
                background-position: 0 0;
            }
            100% {
                background-position: 200% 0;
            }
        }

        h1, h2, h3, p, li {
            margin: 0;
            padding: 0;
        }

        h1 {
            font-size: 28px;
            margin-bottom: 10px;
        }

        ul, ol {
            list-style: none;
            margin-bottom: 15px;
        }

        ul li, ol li {
            margin-bottom: 5px;
        }

        a {
            color: #000000; /* Cinza escuro: #333333 */
            text-decoration: none;
            cursor: pointer;
        }

        #guild-info-container,
        #journal-container {
            display: none;
        }

        .button-container {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }

        .action-button {
            flex: 1;
            margin-right: 0.30cm; 
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            background-color: #444444; /* Cinza escuro: #444444 */
            color: #ffffff;
        }

        #accept-btn {
            margin-right: 10px;
        }

        #name-input {
            width: calc(100% - 20px);
            padding: 10px;
            margin-bottom: 10px;
            box-sizing: border-box;
        }

        #journal-btn {
            background-color: #444444; /* Vermelho: #d9534f */
        }

        #view-guild-info-btn,
        #journal-btn {
            margin-top: 10px;
        }
    </style>
    <title>Convite para Guilda</title>
</head>
<body>

<div id="invite-container">
    <div class="gradient-border"></div>
    <h1>Guilda Ravenclaw - Black Desert Online</h1>
    <p>Caro(a) Aventureiro(a),</p>
    <p>Você está cordialmente convidado(a) a se juntar à nossa guilda em Black Desert Online. Estamos em busca de magos e bruxas destemidos(as) que desejam explorar os mistérios do mundo mágico de Black Desert.</p>
    <label for="name-input">Qual seu nome, jovem bruxo(a)?</label>
    <input type="text" id="name-input" style="width: calc(100% - 20px); padding: 8px; box-sizing: border-box;">
    <div class="button-container">
        <button id="accept-btn" class="action-button" onclick="showGuildInfo()">Aceitar Convite</button>
    </div>
</div>

<div id="guild-info-container">
    <div class="gradient-border"></div>
    <h2>Bem-vindo à Guilda Ravenclaw do Black Desert!</h2>
    
    <p><strong>Venha se juntar a nós!</strong></p>
    <ul>
        <li>🌙 Uma comunidade pacífica no Black Desert Online. 🌟</li>
        <li>🗡️ Somos Full PVE, não pedimos e nem recebemos guerras!</li>
        <li>🌐 Explore tranquilamente o vasto mundo de BDO!</li>
        <li>🤝 Faça amizades conosco no Discord e WhatsApp!</li>
        <li>📈 Avance em missões e conquistas!</li>
        <li>💥 Realizamos eventualmente Dungevons, principalmente em temporada!</li>
    </ul>
    <p><strong>Não temos requisitos de Admissão!</strong></p>
    <ul>
        <li>. Somos sua Hogwarts no Black Desert, não pedimos nível ou GS</li>
        <li>. Não temos obrigações com quests, boss guild ou guerra</li>
        <li>. Nossa única ambição é te ajudar a crescer e prosperar</li>
    </ul>
    <p><strong>Como se juntar:</strong></p>
    <ol>
        <li>Procure por "Ravenclaw" no menu de Guildas em BDO.</li>
        <li>Procure um de nossos oficiais! Nome das famílias disponíveis no Discord.</li>
        <li>Entre em contato conosco via Discord: <a href="[https://discord.gg/HaWxqf79Cz]" target="_blank">Discord-Ravenclaw</a></li>
    </ol>
    <p id="welcome-message">Seja parte da Ravenclaw e se divirta conosco!</p>
    <div class="button-container">
        <button id="view-guild-info-btn" class="action-button" onclick="hideGuildInfo()">Voltar para o Convite</button>
        <button id="journal-btn" class="action-button" onclick="showJournal()">Eventos e novidades</button>
    </div>
</div>

<div id="journal-container">
    <div class="gradient-border"></div>
    <h2>Jornal BDO Diário</h2>
    <p>Leia as últimas notícias do Black Desert Online no site do Garmoth!</p>
    <a href="https://garmoth.com" target="_blank">Confira aqui</a>
    <div class="button-container">
        <button class="action-button" onclick="hideJournal()">Voltar para o Convite</button>
    </div>
</div>

<script>
    function showGuildInfo() {
        var playerName = document.getElementById('name-input').value;
        if (playerName) {
            document.getElementById('invite-container').style.display = 'none';
            document.getElementById('guild-info-container').style.display = 'block';
            document.getElementById('welcome-message').innerHTML = 'Bem-vindo(a) à Ravenclaw, ' + playerName + '!';
        } else {
            alert('Por favor, informe seu nome antes de aceitar o convite.');
        }
    }

    function hideGuildInfo() {
        document.getElementById('invite-container').style.display = 'block';
        document.getElementById('guild-info-container').style.display = 'none';
    }

    function showJournal() {
        document.getElementById('guild-info-container').style.display = 'none';
        document.getElementById('journal-container').style.display = 'block';
    }

    function hideJournal() {
        document.getElementById('guild-info-container').style.display = 'block';
        document.getElementById('journal-container').style.display = 'none';
    }
</script>

</body>
</html>
