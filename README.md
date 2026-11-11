# JoseMartini-atividades-html_basico
Página web sobre o filme Sonhos de Trem (2025), desenvolvida com HTML5 e CSS3 para a disciplina de Desenvolvimento de Interfaces. O projeto apresenta sinopse, elenco, direção e capa do filme, utilizando HTML semântico, Flexbox, Grid e design responsivo. 
C:\Users\jose.martini\Downloads\app.js\index.html  

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Sonhos de Trem | Página do Filme</title>

    <link rel="stylesheet" href="estilo.css">
</head>

<body>

    <header class="cabecalho">
        <h1>Sonhos de Trem</h1>
        <p>Uma história sobre a vida, o amor e as perdas.</p>

        <nav>
            <ul>
                <li><a href="#inicio">Início</a></li>
                <li><a href="#sinopse">Sinopse</a></li>
                <li><a href="#elenco">Elenco</a></li>
                <li><a href="#diretor">Diretor</a></li>
            </ul>
        </nav>
    </header>

    <main>

        <section id="inicio" class="destaque">

            <article class="capa">
                <img
                    src="https://image.tmdb.org/t/p/original/8a8a8a8a8a8a8a8a8a8a8a8a8a8a8a8.jpg"
                    alt="Capa do filme Sonhos de Trem"
                    onerror="this.style.display='none';"
                >
            </article>

            <article class="informacoes">
                <h2>Sonhos de Trem</h2>

                <p>
                    <strong>Título original:</strong> Train Dreams
                </p>

                <p>
                    <strong>Ano:</strong> 2025
                </p>

                <p>
                    <strong>Gênero:</strong> Drama
                </p>

                <p>
                    <strong>Duração:</strong> 102 minutos
                </p>

                <p>
                    <strong>Classificação:</strong> 14 anos
                </p>

                <p class="descricao">
                    Um filme emocionante que retrata a trajetória de um
                    homem em meio às transformações dos Estados Unidos
                    no início do século XX.
                </p>
            </article>

        </section>

        <section id="sinopse" class="conteudo">

            <h2>Sinopse</h2>

            <article>
                <p>
                    Sonhos de Trem acompanha a vida de Robert Grainier,
                    um trabalhador que participa da construção e expansão
                    das ferrovias nos Estados Unidos no início do século XX.
                    Durante sua jornada, ele enfrenta longos períodos de
                    afastamento da família, dificuldades e perdas pessoais.
                </p>

                <p>
                    Ao longo da história, Robert precisa lidar com o amor,
                    a solidão e as mudanças de um mundo em transformação.
                    O filme apresenta uma reflexão sobre a vida, a natureza
                    e a importância das pequenas experiências humanas.
                </p>
            </article>

        </section>

        <section id="elenco" class="conteudo">

            <h2>Elenco Principal</h2>

            <div class="elenco-container">

                <article class="ator">
                    <h3>Joel Edgerton</h3>
                    <p>Robert Grainier</p>
                </article>

                <article class="ator">
                    <h3>Felicity Jones</h3>
                    <p>Gladys Grainier</p>
                </article>

                <article class="ator">
                    <h3>William H. Macy</h3>
                    <p>Arn Peeples</p>
                </article>

                <article class="ator">
                    <h3>Kerry Condon</h3>
                    <p>Claire Thompson</p>
                </article>

                <article class="ator">
                    <h3>Nathaniel Arcand</h3>
                    <p>Ignatius Jack</p>
                </article>

                <article class="ator">
                    <h3>Clifton Collins Jr.</h3>
                    <p>Boomer</p>
                </article>

            </div>

        </section>

        <section id="diretor" class="conteudo">

            <h2>Direção</h2>

            <article class="diretor">
                <h3>Clint Bentley</h3>

                <p>
                    Clint Bentley é o diretor de Sonhos de Trem.
                    Ele também participou da elaboração do roteiro
                    ao lado de Greg Kwedar. O filme é baseado na obra
                    literária de Denis Johnson.
                </p>
            </article>

        </section>

    </main>

    <footer class="rodape">
        <p>Projeto desenvolvido para a disciplina de Desenvolvimento de Interfaces.</p>
        <p>Filme: Sonhos de Trem (2025)</p>
    </footer>

</body>
</html>   

<img
    src="https://www.cinepasseio.org/painel/uploads/698de85ce5374.jpg"
    alt="Pôster oficial do filme Sonhos de Trem"
>

/* Variáveis de cores, fontes e espaçamentos */
:root {
    --cor-fundo: #101812;
    --cor-secundaria: #1e3025;
    --cor-destaque: #b6a477;
    --cor-texto: #f5f1e8;
    --cor-texto-secundario: #c7c7bd;

    --fonte-principal: Arial, Helvetica, sans-serif;

    --espacamento-pequeno: 10px;
    --espacamento-medio: 20px;
    --espacamento-grande: 40px;

    --borda-arredondada: 12px;
}

/* Configurações gerais */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: var(--fonte-principal);
    background-color: var(--cor-fundo);
    color: var(--cor-texto);
    line-height: 1.7;
}

/* Cabeçalho */
.cabecalho {
    background-color: var(--cor-secundaria);
    text-align: center;
    padding: var(--espacamento-grande);
    border-bottom: 3px solid var(--cor-destaque);
}

.cabecalho h1 {
    color: var(--cor-destaque);
    font-size: 38px;
    margin-bottom: var(--espacamento-pequeno);
}

.cabecalho p {
    color: var(--cor-texto-secundario);
}

/* Menu de navegação */
nav ul {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: var(--espacamento-medio);
    list-style: none;
    margin-top: var(--espacamento-medio);
}

nav a {
    color: var(--cor-texto);
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

nav a:hover {
    color: var(--cor-destaque);
}

/* Conteúdo principal */
main {
    max-width: 1100px;
    margin: auto;
    padding: var(--espacamento-grande);
}

/* Destaque do filme */
.destaque {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: var(--espacamento-grande);
    flex-wrap: wrap;
    margin-bottom: 50px;
}

.capa {
    flex: 1;
    min-width: 250px;
    max-width: 350px;
}

.capa img {
    width: 100%;
    height: auto;
    display: block;
    border-radius: var(--borda-arredondada);
    box-shadow: 0 5px 20px rgba(0, 0, 0, 0.5);
}

.informacoes {
    flex: 1;
    min-width: 250px;
}

.informacoes h2 {
    color: var(--cor-destaque);
    font-size: 32px;
    margin-bottom: var(--espacamento-medio);
}

.informacoes p {
    margin-bottom: var(--espacamento-pequeno);
}

.descricao {
    margin-top: var(--espacamento-medio);
    color: var(--cor-texto-secundario);
}

/* Seções */
.conteudo {
    background-color: var(--cor-secundaria);
    padding: 30px;
    margin-bottom: var(--espacamento-grande);
    border-radius: var(--borda-arredondada);
}

.conteudo h2 {
    color: var(--cor-destaque);
    font-size: 26px;
    margin-bottom: var(--espacamento-medio);
    border-bottom: 2px solid var(--cor-destaque);
    padding-bottom: var(--espacamento-pequeno);
}

.conteudo p {
    color: var(--cor-texto-secundario);
    margin-bottom: var(--espacamento-pequeno);
}

/* Elenco */
.elenco-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: var(--espacamento-medio);
}

.ator {
    background-color: var(--cor-fundo);
    padding: var(--espacamento-medio);
    border-radius: var(--borda-arredondada);
    text-align: center;
    border: 1px solid var(--cor-destaque);
    transition: transform 0.3s;
}

.ator:hover {
    transform: translateY(-5px);
}

.ator h3 {
    color: var(--cor-destaque);
    margin-bottom: var(--espacamento-pequeno);
}

.ator p {
    margin: 0;
}

/* Diretor */
.diretor {
    padding: var(--espacamento-pequeno);
}

.diretor h3 {
    color: var(--cor-destaque);
    margin-bottom: var(--espacamento-pequeno);
}

/* Rodapé */
.rodape {
    background-color: var(--cor-secundaria);
    text-align: center;
    padding: 30px;
    border-top: 3px solid var(--cor-destaque);
}

.rodape p {
    color: var(--cor-texto-secundario);
    margin-bottom: 5px;
}

/* Responsividade para celulares */
@media (max-width: 600px) {

    .cabecalho h1 {
        font-size: 28px;
    }

    main {
        padding: var(--espacamento-medio);
    }

    .destaque {
        flex-direction: column;
        text-align: center;
    }

    .capa {
        max-width: 280px;
    }

    nav ul {
        gap: 12px;
    }

    .conteudo {
        padding: var(--espacamento-medio);
    }
}



