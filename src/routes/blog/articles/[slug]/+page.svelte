<script>
    import { page } from '$app/stores';

    let slug = $page.params.slug;
    const articles = import.meta.glob('..//*.svelte');
    const loadArticle = articles[`../${slug}.svelte`]?.();
</script>

<main>
    {#if loadArticle}
        {#await loadArticle}
            <p>Chargement...</p>
        {:then article}
            <article.default />
        {/await}
    {:else}
        <p>Article introuvable.</p>
    {/if}
</main>

<style>
    main {
        padding: 20px;
        color: #fff;
    }
</style>
