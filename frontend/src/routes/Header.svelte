<script>
	import { page } from '$app/stores';
</script>

<header>
	<nav>
		<div class="corner">
			<a class="app-logo" href="/">s<span>up</span>port</a>
		</div>

		<ul>
			<li aria-current={$page.url.pathname === '/dashboard' ? 'page' : undefined}>
				<a href="/dashboard">Dashboard</a>
			</li>
			<li aria-current={$page.url.pathname === '/tickets' ? 'page' : undefined}>
				<a href="/tickets">Tickets</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
		</ul>

		<div class="corner right">
			<a href="/">User</a>
		</div>
	</nav>
</header>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Gugi&display=swap');

	.app-logo {
		font-size: 1.2rem;
		font-family: 'Gugi', cursive;
		color: var(--accent-color-0);
	}

	.corner {
		width: inherit;
	}

	.right {
		display: flex;
		justify-content: flex-end;
	}

	header {
		display: flex;
		justify-content: center;
	}
	
	nav {
		width: 100%;
		display: flex;
		justify-content: space-between;
		background: var(--color-bg-dark);
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 4em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--color-bg-dark);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page'] a {
		color: var(--accent-color-0);
		text-decoration: underline var(--accent-color-0);
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-bg-secondary);
		font-weight: bold;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	span {
		color: var(--color-bg-secondary);
	}

	a:hover {
		color: var(--accent-color-0);
	}
</style>
