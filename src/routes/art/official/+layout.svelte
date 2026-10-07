<script>
	import { page } from "$app/state";
	import "$lib/assets/shared.css";
    import HorizontalNavbar from "$lib/navbarH.svelte";
	let { children } = $props();
    
    const navItems = [
		{ href: "/art/official", label: "Hellsinker Artwork"},
		{ href: "/art/official/other", label: "Misc Artwork"},
	];

</script>

<main class="app-content">
    <HorizontalNavbar {navItems}/>
    
	{@render children()}
</main>
