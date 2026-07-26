<main>
    <h1>Muninn, mon organisateur de projets fait main.</h1>
    <p class="date">Publié le 26 juillet 2026</p>

    <p>Je développe actuellement Muninn, un organisateur de projets desktop, en solo.</p>
    <p>L'idée m'est venue en découvrant <span class="gras">Keepio</span>, une application développée par <span class="surlinage">Carolane Lefebvre</span> pensée pour organiser ses idées.</p>
    <p>Ça m'a donné envie d'avoir mon propre outil, pensé cette fois pour organiser mes projets et suivre leur avancement.</p>


    <h2>1. Le choix du nom : Muninn</h2>
    <p>Trouver le bon nom n'a pas été immédiat. J'ai exploré plusieurs pistes : des figures mythologiques, des jeux de mots... Puis je suis tombé sur Muninn, l'un des deux corbeaux d'Odin dans la mythologie nordique.</p>
    <p>Hugin représente la pensée, Muninn la mémoire. Et c'est là que tout a fait sens : un organisateur de projets, au fond, <br>c'est exactement ça - un outil de mémoire. Il garde en tête ce qu'on doit faire, où on en est, ce qu'on a déjà accompli.</p>

    <h2>2. Les choix techniques</h2>
    <p>Faire une application desktop plutôt qu'un simple site web, c'était important pour moi. Ça permet à Muninn de tourner directement sur l'ordinateur, sans dépendre d'un navigateur ou d'une connexion internet, avec un accès plus direct aux fichiers et au système. C'était aussi l'occasion de sortir de ma zone de confort purement web, et d'apprendre à construire un vrai produit installable, avec ses propres contraintes (packaging, mises à jour, performances).</p>
    <p>J'ai choisi Electron plutôt que Tauri pour rester sur une stack que je maîtrise déjà : HTML, CSS, TypeScript et Svelte. Pas besoin d'apprendre le Rust en plus de me lancer dans mon premier vrai projet desktop. Electron a aussi l'avantage d'être bien documenté et très utilisé, ce qui aide quand on avance seul sur ce genre de projet.</p>

    <h2>Source :</h2>
    <div class="source">
        <a href="https://carolanelefebvre.com/fr">Carolane Lefebvre</a>
        <a href="https://keepio.fr/">Keepio</a>
    </div>
</main>

<style>
    main {
        line-height: 1.6;
    }

    h1 {
        font-size: 1.8rem;
        margin-bottom: 0.2rem;
    }

    .date {
        color: #888;
        font-size: 0.9rem;
        margin-bottom: 1.5rem;
    }

    h2 {
        font-size: 1.3rem;
        margin-top: 1.5rem;
        text-decoration: underline;
    }

    .surlinage {
        text-decoration: underline;
    }

    .gras {
        font-weight: bold;
    }

    .source {
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }

    .source a {
        text-decoration: none;
        color: white;
        font-weight: bold;
    }

    .source a:hover {
        text-decoration: underline;
    }
</style>
