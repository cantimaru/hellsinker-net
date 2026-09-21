<script>
	import { page } from "$app/state";
	import "$lib/assets/shared.css";
    import HorizontalNavbar from "$lib/horizontalNavbar.svelte";
	let { children } = $props();
    
    const navItems = [
		{ href: "/music/tracks", label: "Release"},
		{ href: "/music/unused", label: "Unused"},
		{ href: "/music/0.95", label: "0.95 Trial"},
	];

</script>

<main class="app-content">
    <HorizontalNavbar {navItems}/>
    
	{@render children()}
</main>
