<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mundo dos Quadrinhos</title>
    <link rel="stylesheet" href="pg.css">
</head>
<body>
    <header class="cabecalho">
        <h1>Mundo dos Quadrinhos</h1>
        <p>Seu portal sobre o universo das HQs</p>
    </header>
    
    <nav class="menu">
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Heróis</a></li>
            <li><a href="#">Vilões</a></li>
            <li><a href="#">Clássicos</a></li>
            <li><a href="#">Contato</a></li>
        </ul>
    </nav>
    
    <main class="principal">
        <section class="destaque">
            <h2>Destaque do Dia</h2>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSqf7ogbib2gUKlOLcT_jqY5Gaa_RYx7fzINw&s" alt="Capa do quadrinho em destaque desta semana" class="imagem-destaque">
            <p>Conheça a nova edição da saga que está revolucionando o universo dos quadrinhos!</p>
            <button class="btn-leia-mais">Leia Mais</button>
        </section>
        
        <section class="recomendados">
            <h2>Recomendações da Semana</h2>
            <ul>
                <li>Batman: Ano Um - Frank Miller</li>
                <li>Watchmen - Alan Moore</li>
                <li>Maus - Art Spiegelman</li>
                <li>Persépolis - Marjane Satrapi</li>
            </ul>
        </section>
        
        <section class="curiosidades">
            <h2>Você Sabia?</h2>
            <div class="caixa-curiosidade">
                <p>O primeiro quadrinho da Marvel foi publicado em 1939, chamado Marvel Comics #1.</p>
            </div>
        </section>
        
        <section class="lancamentos">
            <h2>Próximos Lançamentos</h2>
            <div class="grid-lancamentos">
                <div class="lancamento">
                    <h3>Novembro</h3>
                    <p>Nova saga do Homem-Aranha</p>
                </div>
                <div class="lancamento">
                    <h3>Dezembro</h3>
                    <p>Especial de Natal da Turma da Mônica</p>
                </div>
                <div class="lancamento">
                    <h3>Janeiro</h3>
                    <p>Novo arco dos X-Men</p>
                </div>
            </div>
        </section>
    </main>
    
    <footer class="rodape">
        <p>&copy; 2023 Mundo dos Quadrinhos - Todos os direitos reservados</p>
        <div class="redes-sociais">
            <a href="#">Facebook</a> | 
            <a href="#">Instagram</a> | 
            <a href="#">Twitter</a>
        </div>
    </footer>
</body>
</html>

body {
    font-family: 'Comic Sans MS', cursive, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f5f5f5;
    color: #333;
    line-height: 1.6;
}

/* Paleta de cores (4 cores principais) */
:root {
    --cor-primaria: #e63946; /* Vermelho heroico */
    --cor-secundaria: #1d3557; /* Azul profundo */
    --cor-clara: #f1faee; /* Fundo claro */
    --cor-destaque: #ffbe0b; /* Amarelo de destaque */
}

/* Header */
.cabecalho {
    background-color: var(--cor-primaria);
    color: white;
    text-align: center;
    padding: 2rem;
    border-bottom: 5px solid var(--cor-destaque);
}

.cabecalho h1 {
    margin: 0;
    font-size: 2.5rem;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
}

/* Menu de navegação */
.menu {
    background-color: var(--cor-secundaria);
    padding: 1rem 0;
}

.menu ul {
    display: flex;
    justify-content: space-around;
    list-style: none;
    padding: 0;
    margin: 0;
}

.menu a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    padding: 0.5rem 1rem;
    transition: all 0.3s ease;
}

.menu a:hover {
    background-color: var(--cor-destaque);
    color: var(--cor-secundaria);
    border-radius: 5px;
}

/* Conteúdo principal */
.principal {
    display: grid;
    grid-template-columns: 1fr;
    gap: 2rem;
    padding: 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

/* Seção de destaque */
.destaque {
    background-color: white;
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
}

.imagem-destaque {
    max-width: 100%;
    height: auto;
    border: 3px solid var(--cor-secundaria);
    border-radius: 5px;
    margin: 1rem 0;
}

.btn-leia-mais {
    background-color: var(--cor-destaque);
    color: var(--cor-secundaria);
    border: none;
    padding: 0.8rem 1.5rem;
    font-weight: bold;
    border-radius: 5px;
    cursor: pointer;
    transition: transform 0.3s, background-color 0.3s;
}

.btn-leia-mais:hover {
    background-color: var(--cor-primaria);
    color: white;
    transform: scale(1.05);
}

/* Seção de recomendados */
.recomendados {
    background-color: var(--cor-clara);
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.recomendados ul {
    list-style-type: none;
    padding: 0;
}

.recomendados li {
    padding: 0.5rem 0;
    border-bottom: 1px dashed var(--cor-secundaria);
}

.recomendados li:last-child {
    border-bottom: none;
}

/* Seção de curiosidades */
.curiosidades {
    background-color: var(--cor-secundaria);
    color: white;
    padding: 1.5rem;
    border-radius: 10px;
    text-align: center;
}

.caixa-curiosidade {
    background-color: rgba(255, 255, 255, 0.1);
    padding: 1rem;
    border-radius: 5px;
    animation: fadeIn 2s ease-in;
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

/* Seção de lançamentos */
.lancamentos {
    background-color: white;
    padding: 1.5rem;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.grid-lancamentos {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
}

.lancamento {
    background-color: var(--cor-clara);
    padding: 1rem;
    border-radius: 5px;
    border-left: 4px solid var(--cor-primaria);
    transition: transform 0.3s;
}

.lancamento:hover {
    transform: translateY(-5px);
}

/* Rodapé */
.rodape {
    background-color: var(--cor-secundaria);
    color: white;
    text-align: center;
    padding: 1.5rem;
    margin-top: 2rem;
}

.redes-sociais a {
    color: var(--cor-destaque);
    text-decoration: none;
    margin: 0 0.5rem;
}

/* Responsividade */
@media (min-width: 768px) {
    .principal {
        grid-template-columns: 2fr 1fr;
    }
    
    .destaque {
        grid-column: 1 / span 2;
    }
}

