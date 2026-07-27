<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<header>
	<nav>
		<div class="menu">
			<a href="/"><img src="{favicon}" alt=""></a>
			<a href="/programmes" class="menu-item-icon"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-code"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M7 8l-4 4l4 4" /><path d="M17 8l4 4l-4 4" /><path d="M14 4l-4 16" /></svg>Mes programmes</a>
			<a href="/cursus" class="menu-item-icon"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-school"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M22 9l-10 -4l-10 4l10 4l10 -4v6" /><path d="M6 10.6v5.4a6 3 0 0 0 12 0v-5.4" /></svg>Cursus</a>
			<a href="/blog" class="menu-item-icon"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-notebook"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M6 4h11a2 2 0 0 1 2 2v12a2 2 0 0 1 -2 2h-11a1 1 0 0 1 -1 -1v-14a1 1 0 0 1 1 -1m3 0v18" /><path d="M13 8l2 0" /><path d="M13 12l2 0" /></svg>Blog</a>
			<a href="/contact" class="menu-item-icon"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-contract"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M8 21h-2a3 3 0 0 1 -3 -3v-1h5.5" /><path d="M17 8.5v-3.5a2 2 0 1 1 2 2h-2" /><path d="M19 3h-11a3 3 0 0 0 -3 3v11" /><path d="M9 7h4" /><path d="M9 11h4" /><path d="M18.42 12.61a2.1 2.1 0 0 1 2.97 2.97l-6.39 6.42h-3v-3l6.42 -6.39" /></svg>Contact</a>
		</div>
		<div class="social">
			<a href="https://www.linkedin.com/in/wilstan-sanquer/" aria-label="LinkedIn" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-brand-linkedin"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M8 11v5" /><path d="M8 8v.01" /><path d="M12 16v-5" /><path d="M16 16v-3a2 2 0 1 0 -4 0" /><path d="M3 7a4 4 0 0 1 4 -4h10a4 4 0 0 1 4 4v10a4 4 0 0 1 -4 4h-10a4 4 0 0 1 -4 -4l0 -10" /></svg></a>
			<a href="https://github.com/wilstan-sanquer" aria-label="Github" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-brand-github"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5" /></svg></a>
			<a href="https://gitlab.com/wilstan-sanquer" aria-label="Gitlab" target="_blank"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-brand-gitlab"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M21 14l-9 7l-9 -7l3 -11l3 7h6l3 -7l3 11" /></svg></a>
			<hr class="hr-vertical">
			<a href="download" aria-label="Download"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-download"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M4 17v2a2 2 0 0 0 2 2h12a2 2 0 0 0 2 -2v-2" /><path d="M7 11l5 5l5 -5" /><path d="M12 4l0 12" /></svg></a>
		</div>
	</nav>
</header>

<main>
	{@render children()}
</main>

<footer>
	<p>Made by <a href="https://github.com/wilstan-sanquer">SAW</a>. Tous droits réservés.</p>
	<a class="legal" href="mentions-legal">Mentions légales</a>
</footer>

<style>
	nav {
		display: flex;
		justify-content: space-between;
		padding-top: 1rem;
		padding-bottom: 1rem;
		align-items: center;
		margin-left: 5px;
		margin-right: 5px;
	}

	.menu {
		display: flex;
		gap: 30px;
		width: 60%;
		align-items: center;
		font-weight: bold;
	}

	.menu a {
		text-decoration: none;
		color: white;
	}

	.menu-item-icon {
		display: flex;
		align-items: center;
		gap: 6px;
		white-space: nowrap;
	}

	.menu a:hover,
	.social a:hover {
        color: #fa3d00;
	}

	.menu img {
		margin: 0;
		padding: 0;
		height: 50px;
		width: auto;
	}

	.social {
		display: flex;
		justify-content: end;
		width: 50%;
		gap: 30px;
	}

	.social a {
		color: white;
	}

	.hr-vertical {
        width: 1px;
        height: 20px;
        background-color: white;
        border: none;
        display: inline-block;
        margin: 0;
        align-self: center;
        flex-shrink: 0;
	}

	footer {
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-top: .75rem;
		margin-bottom: .75rem;
		margin-left: 5px;
		margin-right: 5px;
	}

	footer p {
		color: #8B93A0;
	}

	footer a {
		text-decoration: none;
		color: #8B93A0;
	}

	footer a:hover {
		color: whitesmoke;
	}

	.legal {
		text-decoration: underline;
	}
</style>
