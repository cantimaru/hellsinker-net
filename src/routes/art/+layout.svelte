<script>
	import { page } from "$app/state";
	import "$lib/assets/shared.css";
    import HorizontalNavbar from "$lib/navbarH.svelte";
	let { children } = $props();
    
    const navItems = [
		{ href: "/art/official", label: "Official Artwork"},
		{ href: "/art/fanart", label: "Fanmade Artwork"},
	];

</script>

<main class="app-content">
    <HorizontalNavbar {navItems}/>
    
	{@render children()}
</main>
