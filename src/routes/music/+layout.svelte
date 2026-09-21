<script>
	import { page } from "$app/state";
	import "$lib/assets/shared.css";
	let { children } = $props();

    const navItems = [
		{ href: "/music/tracks", label: "Release"},
		{ href: "/music/unused", label: "Unused"},
		{ href: "/music/0.95", label: "0.95 Trial"},
	];
</script>

<main class="app-content">
    <nav>
        <ul class="flex justify-between">
            {#each navItems as item}
            <li>
                <a href={item.href} aria-current={page.url.pathname === item.href}>{item.label}</a>
            </li>
            {/each}
        </ul>
    </nav>
    
	{@render children()}
</main>
