# local_turistico
Desenvolver uma Landing Page de turismo utilizando apenas HTML e CSS

🏝️ Alagoas: O Paraíso das Águas

Um website estático, responsivo e com foco em design moderno, criado para destacar os principais pontos turísticos do estado de Alagoas, Brasil.

✨ Sobre o Projeto

Este projeto foi desenvolvido como um exercício prático de web design e desenvolvimento front-end, focado em implementar um layout moderno e responsivo utilizando HTML e CSS Puro (sem frameworks CSS como Tailwind ou Bootstrap).

O objetivo principal é apresentar a beleza das praias e atrações de Alagoas, garantindo uma experiência de usuário agradável em qualquer dispositivo.

📋 Lista de Tarefas Concluídas (Checklist)

O projeto cumpre todos os requisitos de design e estrutura propostos no checklist original sugerido pelo desafio da Rocketseat:

    ✅ Criar a estrutura base em HTML

    ✅ Adicionar o título da página no head (ex.: "Alagoas: O Paraíso das Águas")

    ✅ Criar o header com título principal da página

    ✅ Criar a seção de destaque com imagem e texto de introdução apresentando o local

    ✅ Criar uma seção de artigos com 3 pontos turísticos (imagem, título, descrição e link "Saiba mais")

    ✅ Aplicar estilos com CSS (fontes, tamanhos e cores personalizadas)

    ✅ Utilizar imagens com bordas arredondadas e espaçamento

    ✅ Aplicar espaçamentos entre seções

    ✅ Criar o rodapé com créditos e/ou direitos autorais

    ✅ Revisar boas práticas de código (semântica)

🛠️ Tecnologias Utilizadas

Este projeto foi construído apenas com tecnologias web básicas, demonstrando a capacidade do CSS moderno:

    HTML5: Estrutura semântica do conteúdo.

    CSS3 (Puro):

        Utilização de Variáveis CSS (:root) para cores, facilitando a manutenção e a customização.

        Layout Responsivo com uso de media queries.

        Implementação de Grid Layout para a seção de destaques.

Eu desenvolvi esse projeto mas foi corrigido por IA. 

---------------------------------------------------------------------------------------------------------------

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alagoas: O Paraíso das Águas</title>
    <link rel="stylesheet" href="style.css">
    </head>
<body>

    <header class="main-header">
        <div class="container header-container">
            <h1 class="main-title">Alagoas</h1>
            <p class="header-subtitle">O Paraíso das Águas</p>
        </div>
    </header>

    <main class="container main-content">

        <section id="introducao" class="section-intro">
            <h2 class="section-title text-center text-primary-teal">Sua Próxima Viagem Inesquecível</h2>

            <div class="intro-box">
                <figure class="intro-figure">
                    <img class="main-image"
                        src="https://www.locatemporada.com.br/media/615b8d78f07dc97589045011/md"
                        alt="Vista panorâmica da Praia de Ponta Verde"
                        onerror="this.onerror=null;this.src='https://placehold.co/1200x600/0d9488/ffffff?text=Maceio+Mar+Azul'">
                    <figcaption class="image-caption">
                        As piscinas naturais e as águas mornas fazem de Maceió um destino único. Venha conhecer!! 
                    </figcaption>
                </figure>

                <p class="intro-text">
                    Maceió, a capital alagoana, é um convite irrecusável ao descanso e à beleza natural. Conhecida como o "Caribe Brasileiro", a cidade encanta com suas praias de águas mornas e transparentes. Além de ser perfeita para aproveitar junto da família, amigos e aquele amor que você sempre quis encantar. 
                </p>
            </div>
        </section>

        <section id="destaques" class="section-destaques">
            <h2 class="section-title text-center text-dark-teal">Descubra 3 Destinos Imperdíveis em Alagoas</h2>

            <p class="destaques-subtitle">
                De praias urbanas badaladas a refúgios tranquilos, os atrativos de Alagoas são variados e acessíveis.
            </p>

            <div class="grid-destaques">

                <div class="card-destaque">
                    <img src="https://dynamic-media-cdn.tripadvisor.com/media/photo-o/06/5d/08/fe/praia-de-ponta-verde.jpg?w=1600&h=-1&s=1" alt="Ponta Verde" class="card-image">
                    <div class="card-body">
                        <h3 class="card-title">Ponta Verde</h3>
                        <p class="card-description">O coração da orla de Maceió.</p>
                        <a href="#" class="card-link">Saiba mais →</a>
                    </div>
                </div>

                <div class="card-destaque">
                    <img src="https://i0.wp.com/travel.com.br/wp-content/uploads/2021/09/franc%C3%AAs-praia.png?w=2000&ssl=1" alt="Praia do Francês" class="card-image">
                    <div class="card-body">
                        <h3 class="card-title">Praia do Francês</h3>
                        <p class="card-description">Localizada em Marechal Deodoro.</p>
                        <a href="#" class="card-link">Saiba mais →</a>
                    </div>
                </div>

                <div class="card-destaque">
                    <img src="https://d3w13n53foase7.cloudfront.net/medium_49402951_7639_42af_9bfa_6d52d830f1a2_caninde_de_sao_francisco_002_297e634370.jpg" alt="Foz do Rio São Francisco" class="card-image">
                    <div class="card-body">
                        <h3 class="card-title">Foz do Rio São Francisco</h3>
                        <p class="card-description">O encontro do rio com o mar.</p>
                        <a href="#" class="card-link">Saiba mais →</a>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <footer class="main-footer">
        <div class="container text-center">
            <p class="footer-text">Desenvolvido com 💙 para o seu roteiro de viagem | Maceió, Alagoas</p>
        </div>
    </footer>

</body>
</html>

CSS --------------------------------------------------------------------------------------------------------------


:root {
    --primary-teal: #0d9488;
    --light-mint: #ccfbf1;
    --dark-teal: #134e4a;
    --gray-text: #4b5563; 
    --light-bg: #f0fdfa; 
}


body {
    font-family: Arial, sans-serif; 
    color: var(--gray-text);
    background-color: var(--light-bg);
    line-height: 1.5; 
    margin: 0;
    padding: 0;
}

.container {
    max-width: 1000px; 
    margin-left: auto;
    margin-right: auto;
    padding-left: 1rem; 
    padding-right: 1rem; 
}

.text-center {
    text-align: center;
}


.main-header {
    background-color: var(--primary-teal);
    padding-top: 3rem; 
    padding-bottom: 3rem; 
    box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05); 
}

.main-title {
    font-size: 4rem; 
    font-weight: 800; 
    color: white;
    text-align: center;
    margin-bottom: 1rem; 
}

@media (min-width: 768px) {
    .main-title {
        font-size: 6rem; 
    }
}

.header-subtitle {
    font-size: 1.5rem; 
    font-weight: 300; 
    color: var(--light-mint);
    text-align: center;
}


.main-content {
    padding-top: 3rem; 
    padding-bottom: 3rem; 
}

.section-title {
    font-size: 2.25rem; 
    font-weight: 700; 
    margin-bottom: 1rem; 
}
.text-primary-teal { color: var(--primary-teal); }
.text-dark-teal { color: var(--dark-teal); }


.section-intro {
    margin-bottom: 4rem; 
}

.intro-box {
    background-color: white;
    padding: 2.5rem; 
    border-radius: 0.75rem; 
    box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05); 
}

.intro-figure {
    margin-bottom: 1.5rem; 
}


.main-image {
    width: 100%; 
    height: auto; 
    object-fit: cover;
    box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.05);
    transition: transform 0.3s ease; 
    border-radius: 28px; 
}

.main-image:hover {
    transform: scale(1.01); 
}

.image-caption {
    text-align: center;
    margin-top: 0.75rem; 
    color: #6b7280; 
    font-style: italic;
    font-size: 0.875rem; 

}

.intro-text {
    font-size: 1.125rem; 
    line-height: 1.625; 
    color: #374151; 
}


.section-destaques {
    margin-bottom: 4rem; 
}

.destaques-subtitle {
    text-align: center;
    font-size: 1.125rem; 
    margin-bottom: 2.5rem; 
    color: #4b5563; 
    max-width: 48rem; 
    margin-left: auto;
    margin-right: auto;
}

.grid-destaques {
    display: grid;
    grid-template-columns: 1fr; 
    gap: 2rem; 
}

@media (min-width: 768px) {
    .grid-destaques {
        grid-template-columns: repeat(3, 1fr);
    }
}


.card-destaque {
    background-color: white;
    border-radius: 0.75rem; 
    box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.05); 
    padding: 1.25rem; 
    border-top: 4px solid var(--primary-teal); 
    transition: box-shadow 0.3s ease; 
}

.card-destaque:hover {
    box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25); 
}

.card-image {
    width: 100%; 
    height: 12rem; 
    object-fit: cover;
    margin-bottom: 1rem;
    border-radius: 0.5rem; 
}

.card-title {
    font-size: 1.5rem; 
    font-weight: 600; 
    color: var(--primary-teal);
    margin-bottom: 0.5rem; 
}

.card-description {
    color: #374151; 
    margin-bottom: 1rem; 
}

.card-link {
    display: inline-block;
    color: var(--primary-teal);
    font-weight: 600; 
    border-bottom: 1px solid var(--primary-teal);
    text-decoration: none;
    transition: color 0.3s ease;
}

.card-link:hover {
    color: var(--dark-teal);
    border-color: var(--dark-teal);
}


.main-footer {
    background-color: var(--dark-teal);
    padding-top: 1.5rem; 
    padding-bottom: 1.5rem; 
    margin-top: 3rem; 
}

.footer-text {
    color: var(--light-mint);
    font-size: 0.875rem; 
}
