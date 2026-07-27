<script>
</script>

<main>
    <div class="cadre">
        <div class="programmes">
            <h1>Muninn</h1>
            <p>Organisateur de projets desktop avec suivi des tâches et de l'avancement.</p>
            <a href="https://github.com/wilstan-sanquer/muninn" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-brand-github"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5" /></svg>Voir le code source</a>
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

    :global(body) {
        background-color: #1a1a1a;
        margin: 0 15% 10px;
        font-family: "Red Hat Display", sans-serif;
    }

    .cadre {
        font-family: "Share Tech", sans-serif;
        display: flex;
        flex-direction: column;
        text-align: left;
        border-radius: 20px;
        background-color: #2a2a2a;
        height: 530px;
        width: 100%;
        overflow-y: auto;
    }

    .programmes {
        display: flex;
        justify-content: space-between;
        align-items: center;
        border: 1px solid #1a1a1a;
        border-radius: 20px;
        margin: 40px;
        padding: 20px;
        color: white;
        background-color: #1a1a1a;
        animation: fadeInUp 0.6s ease-out both;
        animation-delay: 0.05s;
    }

    .programmes p {
        font-size: 19px;
    }

    .programmes a {
        display: flex;
        border: 1px solid white;
        border-radius: 10px;
        padding: 10px;
        text-decoration: none;
        color: white;
        align-items: center;
        justify-content: center;
        gap: 10px;
    }

    .programmes:hover {
        color: #fa3d00;
        background-color: #3a3a3a;
        border: 1px solid #fa3d00;
    }

    .programmes a:hover {
        border: 1px solid #fa3d00;
        color: #fa3d00;
    }
</style>