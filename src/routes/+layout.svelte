<script>
  import { page } from "$app/state";
  import "$lib/assets/shared.css";
  let { children } = $props();

  import greenSquare from "$lib/assets/top.gif";
  import blueDiamond from "$lib/assets/c_blue.gif";
  import blueArrow from "$lib/assets/p_blue.gif";
  import bannerTop from "$lib/assets/banner_top.png";
  import logo from "$lib/assets/hellsinkernet.png";
</script>

<div class="max-w-212 h-screen m-0 mx-auto">
  <div class="app-grid">
    <header class="app-header">
      <div class="header-logo">
	    <img class="logo" src="{logo}" alt="Hellsinker.net">
	  </div>
    </header>

    <nav class="app-toc">
      <ul class="navList">
        <li>
          <a href="/" aria-current={page.url.pathname === "/"}>
            <img src={greenSquare} width="16" height="16" alt="■" />
            Home
          </a>
        </li>
        <li>
          <a href="/info" aria-current={page.url.pathname === "/info"}
            ><img src={blueDiamond} width="16" height="16" alt="■" />Info</a
          >
        </li>
        <li>
          <a href="/links" aria-current={page.url.pathname === "/links"}
            ><img src={blueArrow} width="16" height="16" alt="■" />Links</a
          >
        </li>
        <li>
          <a href="/story" aria-current={page.url.pathname === "/story"}
            ><img src={blueArrow} width="16" height="16" alt="■" />Game Info</a
          >
        </li>
        <li>
          <a href="/tonnor" aria-current={page.url.pathname === "/tonnor"}
            ><img src={blueDiamond} width="16" height="16" alt="■" />Other
            Tonnor Works</a
          >
        </li>
        <li>
          <a href="/contact" aria-current={page.url.pathname === "/contact"}>
            <img src={blueDiamond} width="16" height="16" alt="■" />Contact</a
          >
        </li>
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
