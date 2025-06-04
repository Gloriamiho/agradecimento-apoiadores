<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Área VIP dos Apoiadores Pokémon</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            /* Degradê de rosa bebê para azul bebê */
            background: linear-gradient(135deg, #FFD1DC 0%, #B0E0E6 100%);
            color: #333;
            overflow-x: hidden; /* Evita rolagem horizontal */
            overflow-y: auto; /* Permite rolagem vertical se o conteúdo for muito longo */
            padding-top: 2rem; /* Adiciona um pouco de padding para o topo em telas menores */
            padding-bottom: 2rem; /* Adiciona um pouco de padding para a base em telas menores */
        }

        .card-container {
            background-color: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 2.5rem;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            text-align: center;
            max-width: 90%;
            width: 700px; /* Aumentado um pouco a largura máxima para acomodar mais texto */
            position: relative;
            z-index: 10;
            animation: fadeInScale 1s ease-out forwards;
            border: 2px solid rgba(255, 255, 255, 0.5);
        }

        @keyframes fadeInScale {
            from {
                opacity: 0;
                transform: scale(0.9);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }

        .title {
            font-size: 2.5rem;
            font-weight: 700;
            color: #E91E63; /* Rosa mais vibrante para o título */
            margin-bottom: 1.5rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
        }

        .subtitle {
            font-size: 1.5rem;
            font-weight: 600;
            color: #2196F3; /* Azul mais vibrante para o subtítulo */
            margin-bottom: 1.5rem;
        }

        .section-heading {
            font-size: 1.8rem;
            font-weight: 700;
            color: #E91E63; /* Rosa vibrante para os títulos de seção */
            margin-top: 2.5rem;
            margin-bottom: 1.5rem;
            text-align: center;
        }

        .content-text {
            font-size: 1.15rem;
            line-height: 1.7;
            color: #555;
            margin-bottom: 1.5rem;
        }

        .highlight {
            font-weight: 700;
            color: #E91E63; /* Rosa vibrante para destaques */
        }

        .list-item {
            font-size: 1.1rem;
            line-height: 1.6;
            color: #444;
            margin-bottom: 0.75rem;
            text-align: left; /* Alinha o texto da lista à esquerda */
            padding-left: 1.5rem; /* Espaçamento para o ícone/bullet */
            position: relative;
        }

        .list-item::before {
            content: '✔️'; /* Ícone para lista de benefícios */
            position: absolute;
            left: 0;
            color: #4CAF50; /* Verde para o checkmark */
            font-weight: bold;
        }

        .channel-item::before {
            content: '🔸'; /* Ícone para lista de canais */
            position: absolute;
            left: 0;
            color: #FFC107; /* Amarelo/Laranja para o diamante */
            font-weight: bold;
        }

        .emoji {
            font-size: 2.5rem;
            margin: 0 0.5rem;
            display: inline-block;
            animation: bounce 2s infinite ease-in-out;
        }

        .emoji-cap { animation-delay: 0.1s; }
        .emoji-magnifying-glass { animation-delay: 0.2s; }
        .emoji-lightning { animation-delay: 0.3s; }
        .emoji-heart { animation-delay: 0.4s; }
        .emoji-paw { animation-delay: 0.5s; } /* Novo emoji para o final */

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        /* Efeitos de fundo com emojis flutuantes */
        .floating-emoji {
            position: absolute;
            font-size: 3rem;
            opacity: 0.3;
            animation: float 15s infinite ease-in-out;
            pointer-events: none;
            z-index: 5;
        }

        .floating-emoji:nth-child(1) { top: 10%; left: 5%; animation-delay: 0s; }
        .floating-emoji:nth-child(2) { top: 20%; right: 10%; animation-delay: 2s; font-size: 2.5rem; }
        .floating-emoji:nth-child(3) { bottom: 15%; left: 15%; animation-delay: 4s; font-size: 3.5rem; }
        .floating-emoji:nth-child(4) { top: 5%; right: 25%; animation-delay: 6s; font-size: 2rem; }
        .floating-emoji:nth-child(5) { bottom: 5%; left: 40%; animation-delay: 8s; }
        .floating-emoji:nth-child(6) { top: 30%; left: 30%; animation-delay: 10s; font-size: 4rem; }
        .floating-emoji:nth-child(7) { bottom: 25%; right: 5%; animation-delay: 12s; }
        .floating-emoji:nth-child(8) { top: 40%; right: 40%; animation-delay: 14s; font-size: 2.8rem; }
        .floating-emoji:nth-child(9) { top: 50%; left: 10%; animation-delay: 1s; font-size: 3.2rem; }
        .floating-emoji:nth-child(10) { bottom: 30%; right: 20%; animation-delay: 3s; font-size: 2.7rem; }
        .floating-emoji:nth-child(11) { top: 15%; left: 60%; animation-delay: 5s; font-size: 3.8rem; }
        .floating-emoji:nth-child(12) { bottom: 10%; left: 70%; animation-delay: 7s; font-size: 2.2rem; }


        @keyframes float {
            0%, 100% { transform: translateY(0) translateX(0) rotate(0deg); }
            25% { transform: translateY(-20px) translateX(10px) rotate(5deg); }
            50% { transform: translateY(0) translateX(0) rotate(0deg); }
            75% { transform: translateY(20px) translateX(-10px) rotate(-5deg); }
        }

        /* Responsividade */
        @media (max-width: 768px) {
            .card-container {
                padding: 1.5rem;
                border-radius: 15px;
            }
            .title {
                font-size: 2rem;
                margin-bottom: 1rem;
            }
            .subtitle {
                font-size: 1.2rem;
                margin-bottom: 1rem;
            }
            .section-heading {
                font-size: 1.5rem;
                margin-top: 2rem;
                margin-bottom: 1rem;
            }
            .content-text, .list-item {
                font-size: 1rem;
                line-height: 1.6;
                margin-bottom: 1rem;
            }
            .emoji {
                font-size: 2rem;
            }
            .floating-emoji {
                font-size: 2rem;
            }
        }

        @media (max-width: 480px) {
            .card-container {
                padding: 1rem;
                border-radius: 10px;
            }
            .title {
                font-size: 1.7rem;
            }
            .subtitle {
                font-size: 1rem;
            }
            .section-heading {
                font-size: 1.3rem;
            }
            .content-text, .list-item {
                font-size: 0.9rem;
            }
            .emoji {
                font-size: 1.8rem;
            }
            .floating-emoji {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Emojis flutuantes de fundo para um toque lúdico e expandido -->
    <div class="floating-emoji">✨</div>
    <div class="floating-emoji">💖</div>
    <div class="floating-emoji">💙</div>
    <div class="floating-emoji">⚡</div>
    <div class="floating-emoji">🎉</div>
    <div class="floating-emoji">🧡</div>
    <div class="floating-emoji">🌟</div>
    <div class="floating-emoji">💎</div>
    <div class="floating-emoji">🚀</div>
    <div class="floating-emoji">🐾</div>
    <div class="floating-emoji">🗺️</div>
    <div class="floating-emoji">💡</div>

    <div class="card-container">
        <h1 class="title">🎉✨ Bem-vindo(a) à Área VIP dos Apoiadores! ✨🎉</h1>
        <h2 class="subtitle">Saudações, treinador(a)!
            <span class="emoji emoji-cap">🧢</span>
            <span class="emoji emoji-magnifying-glass">🔍</span>
            <span class="emoji emoji-lightning">⚡</span>
        </h2>
        <p class="content-text">
            Você agora faz parte do nosso seleto grupo de <span class="highlight">Apoiadores Oficiais</span> deste projeto incrível de RPG Pokémon. Sua contribuição é fundamental para que esse sonho aconteça!
            <span class="emoji emoji-heart">🧡</span>
        </p>
        <p class="content-text">
            Ao adquirir nosso <span class="highlight">Livro de Regras</span>, você não só garante uma experiência única de jogo, como também ajuda diretamente no crescimento, desenvolvimento e expansão deste projeto, que é feito com muito amor e dedicação.
        </p>

        <h3 class="section-heading">💎 Por que sua doação é tão importante?</h3>
        <ul>
            <li class="list-item">Ela permite que possamos investir em melhorias do material (revisão, design, ferramentas, atualizações).</li>
            <li class="list-item">Garante que o projeto continue vivo, crescendo e recebendo novos conteúdos.</li>
            <li class="list-item">Valoriza todo o tempo, trabalho e paixão dedicados para criar esse RPG.</li>
        </ul>
        <p class="content-text">
            Você não é apenas um jogador — você é parte da construção desse universo.
        </p>

        <h3 class="section-heading">🚀 Canais Exclusivos que você agora tem acesso:</h3>
        <ul>
            <li class="list-item channel-item">
                <span class="highlight">#avisos-e-enquetes</span> → Onde você receberá informações e anúncios exclusivos antes de todo mundo. Aqui sua voz tem peso! Participe de votações que vão definir conteúdos, nomes, detalhes e até mecânicas futuras.
            </li>
            <li class="list-item channel-item">
                <span class="highlight">#prévias</span> → Conteúdos antecipados, trechos do livro, mecânicas e artes que só os apoiadores verão.
            </li>
            <li class="list-item channel-item">
                <span class="highlight">#chat-dos-apoiadores</span> → Um lounge privado para conversarmos sobre qualquer coisa, trocar ideias, experiências, dúvidas e, claro, muito papo Pokémon!
            </li>
        </ul>

        <h3 class="section-heading">🌟 Se sinta em casa!</h3>
        <p class="content-text">
            Aqui sua presença faz toda a diferença. Muito, muito obrigado por acreditar no nosso projeto.
            <span class="emoji emoji-heart">🧡</span>
            <span class="emoji emoji-paw">🐾</span>
        </p>
        <p class="content-text">
            Se tiver qualquer dúvida, sugestão ou ideia, não hesite em falar no <span class="highlight">#chat-dos-apoiadores</span> ou marcar a staff.
        </p>
        <p class="content-text">
            ➡️ Agora prepare suas Pokébolas... sua jornada como Apoiador começou!
            <span class="emoji">🚀</span>
            <span class="emoji">🌍</span>
            <span class="emoji">✨</span>
        </p>
    </div>
</body>
</html>
