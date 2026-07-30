<script>
	import "../lib/assets/shared.css";
	let { children } = $props();
</script>

<div class="max-w-[45vw] h-screen m-0 mx-auto">
	<div class="app-grid">
		<header class="app-header">
			<h1>Penissinker</h1>
		</header>

		<nav class="app-toc">
			<h2>Navigation thing</h2>
			<ul>
				<li><a href="/">Home</a></li>
				<li><a href="/info">Info</a></li>
				<li><a href="/links">Links</a></li>
				<li><a href="/story">Game Info</a></li>
				<li><a href="/tonnor">Other Tonnor Works</a></li>
				<li><a href="/contact">Contact</a></li>
			</ul>
		</nav>

		<main class="app-content">
			{@render children()}
		</main>

		<footer class="app-footer">
			<p>© 2026 THE CANTI AND CO FOUNDATION</p>
		</footer>
	</div>
</div>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	.app-grid {
		display: grid;
		grid-template-columns: 250px 1fr;
		grid-template-rows: auto 1fr auto;
		min-height: 100vh;
	}

	.app-header {
		grid-column: 1 / -1;
		background-color: #1a1a1a;
		color: white;
		padding: 1rem;
	}

	.app-toc {
		grid-column: 1;
		background-color: #f4f4f4;
		padding: 1rem;
		border-right: 1px solid #ddd;
	}

	.app-content {
		grid-column: 2;
		padding: 2rem;
	}

	.app-footer {
		grid-column: 1 / -1;
		background-color: #222;
		color: #ccc;
		text-align: center;
		padding: 1rem;
	}
</style>

