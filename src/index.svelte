<style>
    div#modal-welcome {
        gap: 10px;
        grid-template-columns: auto;
        grid-template-areas: "header" "main" "footer";
    }
    div#modal-welcome header {
        grid-area: header / header / header / header;
        padding: 0px 2%;
    }
    div#modal-welcome header h2 {
    }
    div#modal-welcome main {
        display: grid;
        grid-area: main / main / main / main;
        grid-template-columns: auto;
        grid-template-areas: "main-aside main-form main-form" "main-aside main-form main-form";
        padding: 0px 2%;
        background-color: rgba(255, 255, 255, 0.8);
    }
    div#modal-welcome main aside {
        grid-area: main-aside / main-aside / main-aside / main-aside;
    }
    div#modal-welcome main aside p {
        font-size: 23px;
    }
    div#modal-welcome main aside span {
        font-size: 60px;
        line-height: 1.1;
    }
    div#modal-welcome main form {
        grid-area: main-form / main-form / main-form / main-form;
    }
    div#modal-welcome main form input {
        width: 50%;
        padding: 5px 10px;
    }
    div#modal-welcome main form input.name {
        margin-right: 5px;
    }
    div#modal-welcome main form input.email {
    }
    div#modal-welcome main form input.size {
    }
    div#modal-welcome main form button {
        background: black;
        color: white;
        padding: 10px 30px;
        text-transform: uppercase;
        border: 1px solid black;
        transition: all 0.3s ease 0s;
    }
    div#modal-welcome main form button:hover {
        background: whitesmoke;
        color: black;
    }
    div#modal-welcome footer {
        grid-area: footer / footer / footer / footer;
        padding: 0px 2%;
    }
</style>

<div id="modal-welcome" class="modal hidden">
    <header>
        <h2>Bem-Vindo</h2>
    </header>
    <main>
        <aside>
            <p>
                Cadastre-se, fique por dentro de nossas novidades, lançamentos e
                na sua primeira compra
            </p>
            <span> Ganhe R$15 </span>
        </aside>
        <form>
            <input class="name" type="text" placeholder="Insira seu Nome" />
            <input class="email" type="email" placeholder="Insira seu Email" />
            <label for="size" class="size">Tamanho</label>
            <select id="size">
                <option>33</option>
                <option>34</option>
                <option>35</option>
            </select>
            <button type="submit" class="cadastroModal">Enviar</button>
        </form>
    </main>
    <footer>
        <span>
            Desconto válido exclusivamente para sua primeira compra no site.
            Oferta não cumulativa com outras promoções. Consulte as condições
            gerais. Ao clicar em "enviar" você aceita nossa
            <a href="/Institucional/politica-de-privacidade">politica de privacidade</a>.
        </span>
    </footer>
</div>
<div id="fvpp-blackout" />
<div id="blackout-overlay" />
