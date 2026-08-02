<script lang='ts'>
	import { page } from "$app/state";
	import "$lib/assets/shared.css";
	let { children } = $props();

	import greenSquare from "$lib/assets/navIco/top.gif"; // reserved for home page link
	import blueDiamond from "$lib/assets/navIco/c_blue.gif"; // for pages with no subpages
	import blueArrow from "$lib/assets/navIco/p_blue.gif"; // for pages with subpages
	import hsSeg from "$lib/assets/navIco/hs_seg.gif";
	import hsGly from "$lib/assets/navIco/hs_glyph.gif";
	import star from "$lib/assets/navIco/rz_star.gif";
	import down from "$lib/assets/navIco/rz_down.gif";
	import flash from "$lib/assets/navIco/hs_flash.gif";
	import life from "$lib/assets/navIco/hs_life.gif";
	import star0 from "$lib/assets/navIco/rz_star0.gif";
	
	import bannerTop from "$lib/assets/banner_top.png";
	import logo from "$lib/assets/hellsinkernet.png"; //
	
	import "$lib/assets/font/fonts.css"
	
	const navItems = [
        { href: "/", label: "Home", icon: greenSquare },
        { href: "/info", label: "Info", icon: blueDiamond },
        { href: "/links", label: "Links", icon: blueArrow },
        { href: "/story", label: "Game Info", icon: star0 },
        { href: "/downloads", label: "Downloads", icon: down },
        { href: "/tonnor", label: "Tonnor Ludography", icon: blueDiamond },
        { href: "/archive", label: "Archives", icon: hsSeg },
        { href: "/fanworks", label: "Fanmade Works", icon: flash },
        { href: "/media", label: "Media", icon: life },
        { href: "#", label: "About HS.Net", icon: hsGly },
        { href: "/contact", label: "Contact Us", icon: star, indent: true},
    ];
</script>

<div class="max-w-212 h-screen m-0 mx-auto">
	<div class="app-grid">
		<header class="app-header">
			<div class="header-logo">
				<img class="logo" src={logo} alt="Hellsinker.net" />
			</div>
		</header>

		<nav class="app-toc">
			<ul class="navList">
				{#each navItems as item}
                    <li style="padding-left: {Number(item.indent ?? 0) * 1.25}rem;">
                        <a href={item.href} aria-current={page.url.pathname === item.href}>
                            <img src={item.icon} width="16" height="16" alt="■" class="object-contain"/>
                            {item.label}
                        </a>
                    </li>
                {/each}
			</ul>
		</nav>

		<main class="app-content">
			{@render children()}
		</main>

		<footer class="app-footer flex justify-between hs-main">
			<p class="text-left">
				<strong>Hellsinker.</strong><br>
				© Ruminant's Whimper
			</p>
			<p class="text-right ml-auto">
				canti * nautichor<br>
				2026 _ Present
			</p>
		</footer>
	</div>
</div>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		overflow-wrap: break-word;

		background-image: url("$lib/assets/bg_ap.jpg");
	}

	.app-grid {
		display: grid;
		grid-template-columns: 250px 1fr;
		grid-template-rows: auto 1fr auto;
		min-height: 100vh;
	}

	.app-header {
		background-image: url("$lib/assets/banner_top.png");
		grid-column: 1 / -1;
		background-color: #1a1a1a;
		color: white;
		padding: 1rem;
	}

	.header-logo {
		padding-top: 4em;
	}

	.logo {
		transform: scale(2);
		transform-origin: left;
		image-rendering: pixelated;
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
		background-color: white;
	}

	.app-footer {
		grid-column: 1 / -1;
		background-color: #222;
		color: #ccc;
		text-align: center;
		padding: 1rem;
	}

	.navList {
		display: flex;
		flex-direction: column;
	}

	.navList a {
		display: flex;
	}
</style>
