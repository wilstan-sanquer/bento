<script>
    let firstname = '';
    let lastname = '';
    let subject = '';
    let email = '';
    let message = '';
    let sent = false;
    let error = false;

    async function handleSubmit(e) {
        e.preventDefault();
        try {
            const res = await fetch('https://formspree.io/f/xqerpgqd', {
                method: 'POST',
                headers: { 'Content-Type': 'application/json' },
                body: JSON.stringify({ firstname, lastname, subject, email, message })
            });
            if (res.ok) {
                sent = true;
            } else {
                error = true;
            }
        } catch {
            error = true;
        }
    }
</script>

<main>
    <div class="cadre">
        {#if sent}
            <p>Merci ! Ton message a bien été envoyé.</p>
        {:else}
            <form onsubmit={handleSubmit}>
                <div class="row">
                    <input type="text" placeholder="Prénom" bind:value={firstname} required>
                    <input type="text" placeholder="Nom" bind:value={lastname} required>
                </div>
                <div class="row">
                    <input type="text" placeholder="Sujet" bind:value={subject} required>
                    <input type="email" placeholder="Email" bind:value={email} required>
                </div>
                <textarea placeholder="Message" bind:value={message} required></textarea>

                <button type="submit">
                    Envoyer
                    <span class="arrow">→</span>
                </button>

                {#if error}
                    <p class="error">Une erreur est survenue, réessaie.</p>
                {/if}
            </form>
        {/if}
    </div>
</main>

<style>
    .cadre {
        border-radius: 20px;
        background-color: #2a2a2a;
        height: 530px;
        width: 100%;
        padding: 40px;
        box-sizing: border-box;
    }

    form {
        display: flex;
        flex-direction: column;
        gap: 16px;
    }

    .row {
        display: flex;
        gap: 16px;
    }

    input, textarea {
        flex: 1;
        background-color: #1e1e1e;
        border: 1px solid #3a3a3a;
        border-radius: 10px;
        padding: 14px;
        color: white;
        font-family: inherit;
        font-size: 15px;
    }

    input::placeholder, textarea::placeholder {
        color: #888;
    }

    textarea {
        min-height: 120px;
        resize: vertical;
    }

    input:focus, textarea:focus {
        outline: none;
        border-color: #d85a30;
    }

    button {
        display: flex;
        align-items: center;
        gap: 8px;
        align-self: flex-start;
        background-color: #d85a30;
        border: none;
        border-radius: 10px;
        padding: 12px 20px;
        color: white;
        font-weight: 600;
        cursor: pointer;
        font-size: 15px;
    }

    button:hover {
        background-color: #c04a24;
    }

    .arrow {
        font-size: 16px;
    }

    .error {
        color: #e24b4a;
    }
</style>