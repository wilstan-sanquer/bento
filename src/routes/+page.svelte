<script>
    //Importation des images pour la page de Bento
    import profil from '$lib/assets/profil.png';
    import logo_archprod from '$lib/assets/logo.png';
    import logo_oracle from '$lib/assets/oracle_logo.png'
    import html from '$lib/assets/techno/HTML.svg';
    import css from '$lib/assets/techno/CSS.svg';
    import javascript from '$lib/assets/techno/JavaScript.svg';
    import java from '$lib/assets/techno/Java.svg';
    import svelte from '$lib/assets/techno/Svelte.svg';
    import tailwind from '$lib/assets/techno/TailwindCSS.svg';
</script>

<main>
    <div class="wrapper">
        <div class="card-perso">
            <h1>Wilstan Sanquer</h1>
            <ul>
                <li>Développeur Junior Frontend & Java</li>
                <li>Étudiant BTS CIEL</li>
            </ul>
        </div>
        <div class="profil">
            <img src="{profil}" alt="PP">
        </div>
        <div class="card-archprod">
            <a href="https://archprod.alwaysdata.net/" target="_blank">
                <h1>Mon <br>Studio <br>de développement</h1>
                <img src="{logo_archprod}" alt="Arch-Prod_logo">
            </a>
        </div>
        <div class="card-oracle">
            <h1>Oracle</h1>
            <img src="{logo_oracle}" alt="Oracle_Bot">
        </div>
        <div class="techno">
            <h1>Mes techno : </h1>
            <div class="techno-icons">
                <img src="{html}" alt="HTML">
                <img src="{css}" alt="CSS">
                <img src="{javascript}" alt="Javascript">
                <img src="{tailwind}" alt="Tailwind">
                <img src="{svelte}" alt="Svelte">
                <img src="{java}" alt="Java">
            </div>
        </div>
    </div>
</main>

<style>
    :global(body) {
        background-color: #1a1a1a;
        margin: 0 15% 10px;
        font-family: "Red Hat Display", sans-serif; 
    }

    .wrapper {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-gap: 10px;
        grid-auto-rows: minmax(100px, auto);
    }

    .card-perso {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: left;
        padding: 20px;
        border-radius: 20px;
        background-color: #2a2a2a;
        grid-row: 1 / 3;
        grid-column: 1 / 3;
    }

    .card-perso h1 {
        margin-left: 0;
        margin-bottom: 10px;
        padding: 0;
        font-size: 45px;
        color: white;
    }

    .card-perso ul {
        list-style-position: inside;
        margin-left: 0;
        padding: 0;
    }

    .card-perso li {
        font-size: 20px;
        color: white;
    }

    .profil {
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 20px;
        background-color: #2a2a2a;
        grid-column: 3 / 5;
        grid-row: 1 / 3;
    }

    .profil img {
        height: 240px;
        width: auto;
    }

    .card-oracle {
        display: flex;
        flex-direction: column;
        border-radius: 20px;
        background: #2A2A2A;
        background: linear-gradient(216deg, rgba(0, 0, 0, 1) 0%, rgba(169, 169, 241, 1) 100%);
        grid-column: 1;
        grid-row: 3 / 5;
        align-items: center;
    }
    
    .card-oracle h1 {
        color: white;
        text-align: center;
    }

    .card-oracle img {
        height: 100px;
        width: auto;
    }

    .card-archprod {
        align-items: center;
        padding: 20px;
        border-radius: 20px;
        background: 2A2A2A;
        background: linear-gradient(165deg, rgba(0, 0, 0, 1) 0%, rgba(22, 145, 114, 1) 100%);
        grid-column: 2 / 5;
        grid-row: 3 / 5;
    }

    .card-archprod a {
        text-decoration: none;
        display: flex;
        justify-content: space-between;
    }

    .card-archprod h1 {
        color: white;
    }

    .card-archprod img {
        height: 150px;
        width: auto;
    }

    .techno {
        display: flex;
        align-items: center;
        border-radius: 20px;
        padding: 10px;
        padding-left: 20px;
        background-color: #2a2a2a;
        grid-row: 5 / 6;
        grid-column: 1 / 5;
    }

    .techno h1 {
        margin-right: 20px;
        color: white;
    }

    .techno-icons {
        display: flex;
        align-items: center;
        gap: 30px;
    }

    .techno-icons img {
        height: 50px;
        width: auto;
    }
</style>