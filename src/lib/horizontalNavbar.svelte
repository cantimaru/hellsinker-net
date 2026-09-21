<script>
	import { page } from "$app/state";
	import "$lib/assets/shared.css";

	let { navItems } = $props();
</script>

<nav>
	<ul class="flex justify-between">
		{#each navItems as item}
			<li>
				<a
					href={item.href}
					aria-current={page.url.pathname === item.href ? "page" : undefined}
				>
					{item.label}
				</a>
			</li>
		{/each}
	</ul>
</nav>