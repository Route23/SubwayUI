<script>
	import { page } from '$app/stores';
	import logo from './svelte-logo.svg';
</script>

<header>
	<nav>
		<ul>
			<li class:active={$page.path === '/'}>
				<a sveltekit:prefetch href="/">
					<div class="yellow black-icon"><i class="material-icons icon">subway</i></div>
				</a>
			</li>
			<li class:active={$page.path === '/docs'}>
				<a sveltekit:prefetch href="/docs">Docs</a>
			</li>
			<!-- <li class:active={$page.path === '/todos'}><a sveltekit:prefetch href="/todos">Todos</a></li> -->
		</ul>
	</nav>
</header>

<style>
	header {
		display: flex;
		padding: 0 32px;
	}

	nav {
		display: flex;
		justify-content: center;
		--background: rgba(255, 255, 255, 0.7);
	}

	svg {
		width: 2em;
		height: 3em;
		display: block;
	}

	path {
		fill: var(--background);
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding-right: 20px;
		color: #fff;
		font-weight: 900;
		font-size: .8735804647362989em;
		text-transform: uppercase;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--accent-color);
	}
	.black-icon {
		color: #000;
		width: 30px;
		height: 30px;
		text-align: center;
		line-height: 42px;
	}
	.yellow {
		background-color: #FCCC0A;
	}
</style>
