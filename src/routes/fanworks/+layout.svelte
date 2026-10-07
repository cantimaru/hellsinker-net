<script>
	import { page } from "$app/state";
	import "$lib/assets/shared.css";
    import HorizontalNavbar from "$lib/navbarH.svelte";
	let { children } = $props();
    
    const navItems = [
		{ href: "/fanworks/doujinshi", label: "Doujinshi"},
		{ href: "/fanworks/fangames", label: "Fan-games"},
		{ href: "/fanworks/music", label: "Fan Compositions"},
	];

</script>

<main class="app-content">
    <HorizontalNavbar {navItems}/>
    
	{@render children()}
</main>
