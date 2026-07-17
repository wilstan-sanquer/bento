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
			<a href="/">Accueil</a>
			<a href="programmes">Mes programmes</a>
			<a href="oracle">Oracle</a>
			<a href="contact">Me contacter</a>
		</div>
		<div class="social">
			<a href="https://www.linkedin.com/in/wilstan-sanquer/" aria-label="LinkedIn"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-brand-linkedin"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M8 11v5" /><path d="M8 8v.01" /><path d="M12 16v-5" /><path d="M16 16v-3a2 2 0 1 0 -4 0" /><path d="M3 7a4 4 0 0 1 4 -4h10a4 4 0 0 1 4 4v10a4 4 0 0 1 -4 4h-10a4 4 0 0 1 -4 -4l0 -10" /></svg></a>
			<a href="https://github.com/wilstan-sanquer" aria-label="Github"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-brand-github"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5" /></svg></a>
			<a href="https://gitlab.com/wilstan-sanquer" aria-label="Gitlab"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-brand-gitlab"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M21 14l-9 7l-9 -7l3 -11l3 7h6l3 -7l3 11" /></svg></a>
			<a href="mailto:wilstan.sanquer@outlook.fr" aria-label="Outlook"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="icon icon-tabler icons-tabler-outline icon-tabler-mail"><path stroke="none" d="M0 0h24v24H0z" fill="none" /><path d="M3 7a2 2 0 0 1 2 -2h14a2 2 0 0 1 2 2v10a2 2 0 0 1 -2 2h-14a2 2 0 0 1 -2 -2v-10" /><path d="M3 7l9 6l9 -6" /></svg></a>
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
		padding-top: 1.75rem;
		padding-bottom: 1.75rem;
	}

	.menu {
		display: flex;
		gap: 30px;
		width: 50%;
	}

	.menu a {
		text-decoration: none;
		color: white;
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

	footer {
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-top: .75rem;
		margin-bottom: .75rem;
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
