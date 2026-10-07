<script>
	import { page } from "$app/state";
	import "$lib/assets/shared.css";
    import HorizontalNavbar from "$lib/navbarH.svelte";
	let { children } = $props();
    
    const navItems = [
		{ href: "/art/fanart", label: "Hellsinker Artwork"},
		{ href: "/art/fanart/other", label: "Misc Artwork"},
	];

</script>

<main class="app-content">
    <HorizontalNavbar {navItems}/>
    <!--TODO: ideally the above navbar for these route-in-route pages would have a different, probably more compact or more sonically fitting design/appearance. but this suffices for now. -->
	{@render children()}
</main>
