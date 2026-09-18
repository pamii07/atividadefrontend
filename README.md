<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Mundo dos Esportes</title>

    <style>
        /* =========================================================
           VARIÁVEIS DA PALETA (Cores Esportivas: Verde & Escuro)
           ========================================================= */
        :root {
            --azul-escuro: #0f2b1d; /* Verde Bem Escuro / Header */
            --azul: #1e7e43;        /* Verde Principal */
            --azul-medio: #27ae60;  /* Verde Destaque */
            --azul-claro: #e8f8f0;  /* Verde Muito Claro */
            --azul-fundo: #f4fbf7;  /* Fundo da Página */
            --branco: #ffffff;
            --texto: #1f2937;
            --borda: #c2e3d0;
            --sombra: rgba(15, 43, 29, 0.12);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.7;
            color: var(--texto);
            background: var(--azul-fundo);
        }

        header {
            background: linear-gradient(135deg, var(--azul-escuro), var(--azul));
            color: var(--branco);
            text-align: center;
            padding: 48px 20px;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        header p {
            max-width: 700px;
            margin: 0 auto;
            opacity: 0.9;
        }

        nav {
            background: var(--branco);
            border-bottom: 1px solid var(--borda);
            box-shadow: 0 2px 8px var(--sombra);
            position: sticky;
            top: 0;
            z-index: 10;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 8px;
            padding: 12px 20px;
        }

        nav a {
            display: block;
            color: var(--azul-escuro);
            text-decoration: none;
            font-weight: bold;
            padding: 8px 16px;
            border-radius: 6px;
        }

        nav a:hover {
            background: var(--azul-claro);
            color: var(--azul);
        }

        main {
            width: min(1100px, 92%);
            margin: 40px auto;
        }

        section {
            background: var(--branco);
            padding: 32px;
            margin-bottom: 30px;
            border: 1px solid var(--borda);
            border-radius: 12px;
            box-shadow: 0 6px 18px var(--sombra);
        }

        h2 {
            color: var(--azul-escuro);
            margin-bottom: 18px;
            font-size: 1.8rem;
        }

        h3 {
            color: var(--azul);
            margin: 24px 0 10px;
        }

        p {
            margin-bottom: 16px;
        }

        ul, ol {
            margin: 12px 0 18px 24px;
        }

        li {
            margin-bottom: 8px;
        }

        .destaque {
            background: var(--azul-claro);
            border-left: 5px solid var(--azul-medio);
            padding: 20px;
            border-radius: 8px;
            margin-top: 20px;
        }

        .galeria {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-top: 20px;
        }

        figure {
            margin: 0;
            background: var(--azul-fundo);
            border: 1px solid var(--borda);
            border-radius: 10px;
            overflow: hidden;
        }

        figure img {
            width: 100%;
            height: 220px;
            object-fit: cover;
            display: block;
        }

        figcaption {
            padding: 12px 14px;
            font-size: 0.9rem;
            color: var(--azul-escuro);
        }

        footer {
            background: var(--azul-escuro);
            color: var(--branco);
            text-align: center;
            padding: 30px 20px;
            margin-top: 50px;
        }

        footer p {
            margin: 4px 0;
        }

        @media (max-width: 700px) {
            header h1 {
                font-size: 2rem;
            }

            section {
                padding: 22px;
            }

            .galeria {
                grid-template-columns: 1fr;
            }

            figure img {
                height: 230px;
            }
        }
    </style>
</head>

<body>

    <header id="inicio">
        <h1>Mundo dos Esportes</h1>
        <p>Acompanhe as principais modalidades, benefícios da atividade física e grandes paixões mundiais.</p>
    </header>

    <nav>
        <ul>
            <li><a href="#inicio">Início</a></li>
            <li><a href="#sobre">Sobre</a></li>
            <li><a href="#modalidades">Modalidades</a></li>
            <li><a href="#galeria">Galeria</a></li>
            <li><a href="#contato">Contato</a></li>
        </ul>
    </nav>

    <main>

        <section id="sobre">
            <h2>A Importância dos Esportes</h2>

            <p>
                A prática regular de esportes vai muito além do alto rendimento. Ela promove a saúde física e mental, previne doenças e estimula a convivência em sociedade.
            </p>

            <p>
                Seja individual ou em equipe, o esporte ensina disciplina, trabalho em time e resiliência diante de desafios diários.
            </p>

            <div class="destaque">
                <p>
                    <strong>Dica de Saúde:</strong> A Organização Mundial da Saúde recomenda pelo menos 150 minutos de atividade física moderada por semana para adultos.
                </p>
            </div>
        </section>

        <section id="modalidades">
            <h2>Modalidades em Destaque</h2>

            <h3>Futebol</h3>
            <p>
                O esporte mais popular do planeta, praticado por milhões de pessoas em todos os continentes. Une culturas e movimenta grandes paixões nacionais.
            </p>

            <h3>Basquetebol</h3>
            <p>
                Dinamismo, agilidade e estratégia definem o basquete, um dos esportes coletivos mais praticados no mundo.
            </p>

            <h3>Benefícios para a Saúde</h3>
            <ul>
                <li>Melhora o sistema cardiovascular.</li>
                <li>Fortalece ossos e músculos.</li>
                <li>Reduz o estresse e melhora a qualidade do sono.</li>
                <li>Desenvolve habilidades sociais e trabalho em grupo.</li>
            </ul>

            <h3>Etapas para começar uma rotina</h3>
            <ol>
                <li>Escolha uma modalidade de que você goste.</li>
                <li>Faça uma avaliação médica prévia.</li>
                <li>Defina metas realistas e progressivas.</li>
            </ol>
        </section>

        <section id="galeria">
            <h2>Galeria Esportiva</h2>

            <p>
                Confira imagens de grandes momentos e modalidades do universo esportivo.
            </p>

            <div class="galeria">

                <figure>
                    <img 
                        src="https://img.freepik.com/fotos-premium/jogador-de-futebol-em-acao-no-fundo-do-estadio-esportivo-chutando-a-bola_760365-11.jpg?w=2000" 
                        alt="Estádio de Futebol"
                    >
                    <figcaption>
                        Futebol: paixão mundial praticada em todos os cantos.
                    </figcaption>
                </figure>

                <figure>
                    <img 
                        src="https://images.unsplash.com/photo-1546519638-68e109498ffc?auto=format&fit=crop&w=800&q=80" 
                        alt="Basquetebol"
                    >
                    <figcaption>
                        Basquetebol: modalidade repleta de ritmo e precisão.
                    </figcaption>
                </figure>

                <figure>
                    <img 
                        src="https://images.unsplash.com/photo-1461896836934-ffe607ba8211?auto=format&fit=crop&w=800&q=80" 
                        alt="Corrida e Atletismo"
                    >
                    <figcaption>
                        Corrida: excelente exercício para a resistência e saúde.
                    </figcaption>
                </figure>

            </div>
        </section>

        <section id="contato">
            <h2>Participe do Nosso Clube</h2>

            <p>
                Quer saber como integrar um grupo esportivo local ou começar os seus treinos hoje mesmo?
            </p>

            <p>
                Entre em contato com a nossa equipe para receber orientações e guias de treino iniciante.
            </p>
        </section>

    </main>

    <footer>
        <p> — Projeto de Esportes</p>
        <p>© 2026 — Mundo dos Esportes</p>
    </footer>

</body>
</html>
