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
					aria-current={page.url.pathname === item.href}
					// this only works for ending hrefs and not intermediary (I.E. /art/official works fine but /art/official/other does not underline the preliminary element on the previous toc (see art gallery and click around, you'll see what i mean))
				>
					{item.label}
				</a>
			</li>
		{/each}
	</ul>
</nav>