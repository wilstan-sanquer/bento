<script>
    import logoStFelix from '$lib/assets/stfelix_logo.png';
</script>

<main>
    <div class="cadre">
        <div class="scroll-wrapper">
            <div class="frise">
                <div class="etape">
                    <img src="{logoStFelix}" alt="St Félix-La Salle" class="logo-ecole">
                    <span class="annee">Sept. 2022 - Juin 2025</span>
                    <div class="trait"></div>
                    <p>Bac Pro<br>Systèmes Électroniques Numériques</p>
                </div>
                <div class="etape">
                    <img src="{logoStFelix}" alt="St Félix-La Salle" class="logo-ecole">
                    <span class="annee">Sept. 2025 - Juin 2027</span>
                    <div class="trait"></div>
                    <p>BTS CIEL<br>Option Informatique et Réseaux</p>
                </div>
            </div>
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
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        border-radius: 20px;
        background-color: #2a2a2a;
        height: 530px;
        width: 100%;
        overflow: hidden;
    }

    .cadre h1, .cadre p {
        color: white;
    }

    .cadre p {
        line-height: 25px;
    }

    .scroll-wrapper {
        width: 80%;
        max-width: 100%;
        overflow-x: auto;
    }

    .frise {
        display: flex;
        align-items: center;
        width: max-content;
        min-width: 100%;
        position: relative;
        padding: 20px 0;
        gap: 60px;
    }

    .logo-ecole {
        width: 50px;
        height: 50px;
        border-radius: 8px;
        object-fit: cover;
    }

    .frise::before {
        content: "";
        position: absolute;
        top: 140px;
        left: 0;
        right: 0;
        height: 2px;
        background-color: #fa3d00;
        z-index: 0;
    }

    .etape {
        flex: 0 0 auto;
        width: 220px;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 10px;
        position: relative;
        z-index: 1;
        animation: fadeInUp 0.6s ease-out both;
    }

    .etape:nth-child(1) { animation-delay: 0.05s; }
    .etape:nth-child(2) { animation-delay: 0.15s; }

    .annee {
        color: #888;
        font-size: 0.9rem;
        white-space: nowrap;
        height: 20px;
        line-height: 20px;
    }

    .trait {
        width: 3px;
        height: 60px;
        background-color: #fa3d00;
    }
</style>