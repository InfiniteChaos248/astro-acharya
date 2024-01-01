<script>
	import { focusedHeader } from '../store.js';
</script>

<header>
	<nav>
		<ul>
			<li aria-current={$focusedHeader == 'h1' ? 'page' : undefined}>
				<a
					class="header-content"
					href="/"
					on:click={() => {
						focusedHeader.set('h1');
					}}
					>HOME</a
				>
			</li>
			<li aria-current={$focusedHeader == 'h2' ? 'page' : undefined}>
				<a
					class="header-content"
                    href="/about"
					on:click={() => {
						focusedHeader.set('h2');
					}}
					>ABOUT US</a>
			</li>
			<li aria-current={$focusedHeader == 'h3' ? 'page' : undefined}>
				<a
					class="header-content"
					href="services"
					on:click={() => {
						focusedHeader.set('h3');
					}}
					>ASTRO SERVICES</a
				>
			</li>
			<li aria-current={$focusedHeader == 'h4' ? 'page' : undefined}>
				<a
					class="header-content"
					href="/contact"
					on:click={() => {
						focusedHeader.set('h4');
					}
					}>CONSULTATION</a
				>
			</li>
		</ul>
	</nav>
</header>

<style>
	nav {
		display: flex;
		justify-content: center;
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
	}

	li {
		position: relative;
		height: 100%;
	}

	li[aria-current='page'] .header-content {
		color: green;
		font-size: 1rem;
	}

	.header-content {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 0.5rem;
		color: var(--color-text);
		font-weight: 700;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	.header-content:hover {
		cursor: pointer;
		font-size: 1rem;
	}
</style>
