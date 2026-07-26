<script></script>
<main>
    <div class="cadre">
        <div class="articles">
            <a href="/blog/articles/muninn-mon-organisateur-de-projets-fait-main"><h1>Muninn, mon organisateur de projets fait main.</h1></a>
            <p class="date">Publié le 26 juillet 2026</p>
        </div>
        <div class="articles">
            <a href="/blog/articles/ce-que-jai-construit-avec-arch-prod"><h1>Ce que j'ai construit avec Arch-Prod.</h1></a>
            <p class="date">Publié le 26 juillet 2026</p>
        </div>
        <div class="articles">
            <a href="/blog/articles/pourquoi-un-portfolio-bento"><h1>Pourquoi j'ai choisi le format Bento pour mon portfolio ?</h1></a>
            <p class="date">Publié le 26 juillet 2026</p>
        </div>
    </div>
</main>
<style>
    @keyframes fadeInUp {
        from {
            opacity: 0;
            transform: translateY(30px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .cadre {
        display: flex;
        flex-direction: column;
        align-items: left;
        text-align: left;
        border-radius: 20px;
        background-color: #2a2a2a;
        height: 530px;
        width: 100%;
        overflow-y: auto;
    }
    .articles {
        margin-top: 40px;
        margin-left: 40px;
        text-align: left;
        animation: fadeInUp 0.6s ease-out both;
    }
    .articles:nth-child(1) { animation-delay: 0.05s; }
    .articles:nth-child(2) { animation-delay: 0.15s; }
    .articles:nth-child(3) { animation-delay: 0.25s; }

    .articles a {
        text-decoration: none;
        color: white;
    }
    .articles a:hover {
        text-decoration: underline;
        color: #fa3d00;
    }
    .articles h1 {
        font-size: 25px;
    }
    .date {
        color: #888;
        font-size: 0.9rem;
    }
</style>
