<script>
    import logo from '$lib/assets/favicon.svg'
    import cv from '$lib/documents/CV_WilstanSanquer_2026.pdf'
</script>

<main>
    <div class="cadre">
        <div class="documents">
            <img src="{logo}" alt="logo">
            <div class="title-documents"><h1>CV <br> Wilstan Sanquer</h1></div>
            <a href="{cv}" target="_blank">Télécharger</a>
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

    .documents {
        animation: fadeInUp 0.6s ease-out both;
    }

    .cadre {
        display: flex;
        flex-direction: column;
        border-radius: 20px;
        height: 530px;
        width: 100%;
    }

    .documents {
        display: flex;
        flex-direction: column;
        width: 25%;
        align-items: center;
        text-align: center;
        justify-content: space-between;
        border: 1px solid #2a2a2a;
        background-color: #2a2a2a;
        border-radius: 20px;
        padding: 20px;
        gap: 20px;
    }

    .documents img {
        width: auto;
        height: 50px;
        border-radius: 10px;
        background-color: #1a1a1a;
        padding: 10px;
    }

    .documents a {
        display: flex;
        border: 1px solid #1a1a1a;
        background-color: #1a1a1a;
        color: white;
        border-radius: 20px;
        height: max-content;
        width: max-content;
        padding: 10px;
        text-decoration: none;
    }

    .documents a:hover {
        background-color: #fa3d00;
    }

    .title-documents {
        color: white;
    }
</style>
