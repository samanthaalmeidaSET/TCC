<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projeto Maquete Extensa</title>
    <style>
        /* Estilos Globais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f4f6f9;
            color: #333;
            line-height: 1.6;
        }

        header {
            background-color: #1e293b;
            color: #ffffff;
            padding: 2rem 1rem;
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        header p {
            font-size: 1.1rem;
            color: #94a3b8;
        }

        /* Container Principal */
        .container {
            max-width: 1100px;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        /* Seções */
        section {
            background: #ffffff;
            padding: 2rem;
            margin-bottom: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
        }

        section h2 {
            color: #0f172a;
            margin-bottom: 1rem;
            border-bottom: 3px solid #3b82f6;
            padding-bottom: 0.5rem;
            display: inline-block;
        }

        /* Galeria de Fotos */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .gallery-item {
            background: #f8fafc;
            border: 1px solid #e2e8f0;
            border-radius: 6px;
            overflow: hidden;
            text-align: center;
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            background-color: #cbd5e1; /* Cor placeholder se não houver imagem */
        }

        .gallery-item p {
            padding: 1rem;
            font-size: 0.95rem;
            font-weight: 500;
        }

        /* Lista de Materiais */
        .materials-list {
            list-style-type: none;
        }

        .materials-list li {
            padding: 0.5rem 0;
            border-bottom: 1px solid #f1f5f9;
            display: flex;
            align-items: center;
        }

        .materials-list li::before {
            content: "✔";
            color: #10b981;
            margin-right: 10px;
            font-weight: bold;
        }

        /* Rodapé */
        footer {
            text-align: center;
            padding: 2rem;
            background-color: #1e293b;
            color: #94a3b8;
            font-size: 0.9rem;
            margin-top: 4rem;
        }

        /* Responsividade */
        @media (max-width: 768px) {
            header h1 { font-size: 2rem; }
            section { padding: 1.5rem; }
        }
    </style>
</head>
<body>

    <!-- Cabeçalho do Site -->
    <header>
        <h1>Apresentação da Maquete</h1>
        <p>Projeto Acadêmico / Profissional de Arquitetura e Engenharia</p>
    </header>

    <div class="container">

        <!-- Sobre o Projeto -->
        <section id="sobre">
            <h2>Sobre o Projeto</h2>
            <p>Este projeto consiste na elaboração de uma maquete física detalhada com o objetivo de representar a viabilidade espacial, a volumetria e a integração com a paisagem do novo complexo urbano. O desenvolvimento buscou aplicar conceitos de sustentabilidade e otimização de materiais.</p>
        </section>

        <!-- Galeria de Imagens -->
        <section id="galeria">
            <h2>Galeria da Maquete</h2>
            <div class="gallery">
                <div class="gallery-item">
                    <!-- Substitua o link abaixo pela sua foto -->
                    <img src="https://placeholder.com" alt="Vista Frontal">
                    <p>Vista Frontal da Estrutura</p>
                </div>
                <div class="gallery-item">
                    <!-- Substitua o link abaixo pela sua foto -->
                    <img src="https://placeholder.com" alt="Vista Superior">
                    <p>Perspectiva Superior (Implantação)</p>
                </div>
                <div class="gallery-item">
                    <!-- Substitua o link abaixo pela sua foto -->
                    <img src="https://placeholder.com" alt="Detalhes Técnicos">
                    <p>Detalhes dos Acabamentos Internos</p>
                </div>
            </div>
        </section>

        <!-- Materiais Utilizados -->
        <section id="materiais">
            <h2>Materiais Utilizados</h2>
            <ul class="materials-list">
                <li>Papel Pluma (Foam board) para a base estrutural</li>
                <li>Acrílico cortado a laser para as fachadas envidraçadas</li>
                <li>MDF para as curvas de nível do terreno</li>
                <li>Vegetação artificial e flocagem para o paisagismo</li>
                <li>Iluminação micro-LED com fiação embutida</li>
            </ul>
        </section>

        <!-- Ficha Técnica / Integrantes -->
        <section id="ficha-tecnica">
            <h2>Ficha Técnica</h2>
            <p><strong>Escala:</strong> 1:50</p>
            <p><strong>Dimensões:</strong> 80cm x 60cm</p>
            <p><strong>Desenvolvido por:</strong> Nome dos Integrantes do Grupo</p>
            <p><strong>Orientação:</strong> Prof. Nome do Orientador</p>
        </section>

    </div>

    <!-- Rodapé -->
    <footer>
        <p>&copy; 2026 - Projeto Maquete. Todos os direitos reservados.</p>
    </footer>

</body>
</html>

