<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mundo das Maquetes | Tutoriais Caseiros</title>
    <style>
        /* --- ESTILOS GERAIS (CSS) --- */
        :root {
            --primary-color: #2c3e50;
            --accent-color: #e67e22;
            --bg-color: #f4f6f7;
            --text-color: #333;
            --card-bg: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        header {
            background-color: var(--primary-color);
            color: white;
            padding: 2rem 1rem;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        header p {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        /* Menu de Filtros */
        .filter-container {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 2rem auto;
            flex-wrap: wrap;
            max-width: 1200px;
            padding: 0 1rem;
        }

        .filter-btn {
            background-color: white;
            border: 2px solid var(--primary-color);
            color: var(--primary-color);
            padding: 0.6rem 1.2rem;
            border-radius: 20px;
            cursor: pointer;
            font-weight: bold;
            transition: all 0.3s ease;
        }

        .filter-btn.active, .filter-btn:hover {
            background-color: var(--primary-color);
            color: white;
        }

        /* Grade de Tutoriais */
        .main-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 1rem 4rem 1rem;
        }

        .grid-tutorials {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        /* Cartão de Tutorial */
        .card {
            background-color: var(--card-bg);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
            display: flex;
            flex-direction: column;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card-img {
            width: 100%;
            height: 200px;
            background-color: #ddd;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            color: #666;
            /* Substitua os fundos abaixo por imagens reais usando src="" se preferir */
            background-size: cover;
            background-position: center;
        }

        .card-content {
            padding: 1.5rem;
            display: flex;
            flex-direction: column;
            flex-grow: 1;
        }

        .tag {
            align-self: flex-start;
            background-color: var(--accent-color);
            color: white;
            font-size: 0.8rem;
            padding: 0.2rem 0.6rem;
            border-radius: 4px;
            margin-bottom: 0.8rem;
            text-transform: uppercase;
            font-weight: bold;
        }

        .card h3 {
            margin-bottom: 0.5rem;
            color: var(--primary-color);
        }

        .card p {
            font-size: 0.95rem;
            color: #555;
            margin-bottom: 1.5rem;
        }

        .btn-read {
            margin-top: auto;
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 0.7rem;
            text-decoration: none;
            border-radius: 4px;
            font-weight: bold;
            transition: background 0.2s;
        }

        .btn-read:hover {
            background-color: #1a252f;
        }

        footer {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 1.5rem;
            position: relative;
            bottom: 0;
            width: 100%;
        }

        /* Responsividade */
        @media (max-width: 600px) {
            header h1 { font-size: 2rem; }
            .filter-container { gap: 5px; }
            .filter-btn { padding: 0.5rem 1rem; font-size: 0.9rem; }
        }
    </style>
</head>
<body>

    <!-- CABEÇALHO -->
    <header>
        <h1>Aprenda Maquetes Caseiras</h1>
        <p>Tutoriais passo a passo usando papelão, materiais reciclados e muita criatividade!</p>
    </header>

    <!-- FILTROS DE CATEGORIA -->
    <div class="filter-container">
        <button class="filter-btn active" onclick="filterCategory('todos')">Todos</button>
        <button class="filter-btn" onclick="filterCategory('escolar')">Projetos Escolares</button>
        <button class="filter-btn" onclick="filterCategory('arquitetura')">Arquitetura</button>
        <button class="filter-btn" onclick="filterCategory('reciclado')">Materiais Reciclados</button>
    </div>

    <!-- CONTEÚDO PRINCIPAL -->
    <main class="main-container">
        <div class="grid-tutorials" id="tutorialsGrid">
            
            <!-- Tutorial 1 -->
            <div class="card" data-category="escolar">
                <div class="card-img" style="background-image: linear-gradient(rgba(0,0,0,0.1), rgba(0,0,0,0.3)), url('https://unsplash.com'); color: white;">Vulcão Escolar</div>
                <div class="card-content">
                    <span class="tag">Escolar</span>
                    <h3>Vulcão de Argila com Erupção</h3>
                    <p>Aprenda a construir um vulcão realista utilizando base de papelão, jornal e argila, com receita caseira para simular a erupção.</p>
                    <a href="#" class="btn-read">Ver Passo a Passo</a>
                </div>
            </div>

            <!-- Tutorial 2 -->
            <div class="card" data-category="arquitetura">
                <div class="card-img" style="background-image: linear-gradient(rgba(0,0,0,0.1), rgba(0,0,0,0.3)), url('https://unsplash.com'); color: white;">Casa Moderna</div>
                <div class="card-content">
                    <span class="tag">Arquitetura</span>
                    <h3>Casa Moderna de Papel Paraná</h3>
                    <p>Crie uma maquete residencial contemporânea com cortes precisos, divisórias internas e dicas de texturização para telhados e gramados.</p>
                    <a href="#" class="btn-read">Ver Passo a Passo</a>
                </div>
            </div>

            <!-- Tutorial 3 -->
            <div class="card" data-category="reciclado">
                <div class="card-img" style="background-image: linear-gradient(rgba(0,0,0,0.1), rgba(0,0,0,0.3)), url('https://unsplash.com'); color: white;">Mini Cidade</div>
                <div class="card-content">
                    <span class="tag">Reciclado</span>
                    <h3>Minicidade com Caixas de Leite</h3>
                    <p>Transforme lixo em arte! Um guia prático para reutilizar caixas de leite e suco para criar prédios, comércios e ruas completas.</p>
                    <a href="#" class="btn-read">Ver Passo a Passo</a>
                </div>
            </div>

            <!-- Tutorial 4 -->
            <div class="card" data-category="escolar">
                <div class="card-img" style="background-image: linear-gradient(rgba(0,0,0,0.1), rgba(0,0,0,0.3)), url('https://unsplash.com'); color: white;">Sistema Solar</div>
                <div class="card-content">
                    <span class="tag">Escolar</span>
                    <h3>Sistema Solar suspenso</h3>
                    <p>Perfeito para a feira de ciências. Use bolinhas de isopor, tintas guache e uma caixa de sapatos preta para simular o espaço sideral.</p>
                    <a href="#" class="btn-read">Ver Passo a Passo</a>
                </div>
            </div>

        </div>
    </main>

    <!-- RODAPÉ -->
    <footer>
        <p>&copy; 2026 Mundo das Maquetes - Feito com criatividade em casa.</p>
    </footer>

    <!-- LOGICA SCRIPT (JAVASCRIPT) -->
    <script>
        function filterCategory(category) {
            // Atualiza a classe ativa nos botões
            const buttons = document.querySelectorAll('.filter-btn');
            buttons.forEach(btn => btn.classList.remove('active'));
            event.target.classList.add('active');

            // Filtra os cartões de tutoriais
            const cards = document.querySelectorAll('.card');
            
            cards.forEach(card => {
                if (category === 'todos') {
                    card.style.display = 'flex';
                } else {
                    if (card.getAttribute('data-category') === category) {
                        card.style.display = 'flex';
                    } else {
                        card.style.display = 'none';
                    }
                }
            });
        }
    </script>
</body>
</html>

