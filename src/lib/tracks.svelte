<script>
	let { tracks } = $props();
</script>

<div class="grid">
	{#each tracks as track}
		{@const bgUrl = `url('/img/music/${track.track}.png')`}
		<article class="track-panel" style="--bg-image: {bgUrl}">
			<h2 class="trackid">{track.track}</h2>
			<h4 class="fan-title">{track.fanTitle}</h4>

			<span class="track-desc">
				{track.desc || "Description goes here."}
				{#if track.motifs}
					<br />Motifs: <i>{track.motifs.join(", ")}</i>
				{/if}
			</span>
		</article>
	{/each}
</div>

<style>
	h1 {
		font-size: 1.6rem;
		margin: 0 0 0.75rem 1rem;
		letter-spacing: 0.04em;
	}

	.grid {
		display: grid;
		grid-template-columns: repeat(2, minmax(0, 1fr));
		gap: 0;
	}

	@media (max-width: 700px) {
		.grid {
			grid-template-columns: 1fr;
		}
	}

	.track-panel {
		position: relative;
		min-height: 140px;
		padding: 0.6rem 0.7rem 0.7rem;
		background-color: #111;
		background-image: linear-gradient(to bottom, #00000000, #000000ff),
			var(--bg-image);
		background-size: cover;
		background-position: center;
		background-repeat: no-repeat;
		border: 1px solid #222;
		box-sizing: border-box;
	}

	.trackid {
		font-size: 1.15rem;
		margin: 0.1rem 0 0.1rem;
		color: white;
	}

	.fan-title {
		margin: 0.05rem 0 0.25rem;
		color: #c9c9d6;
		font-weight: 500;
		line-height: 1.15;
	}

	.track-desc {
		font-size: 0.78rem;
		margin: 0;
		color: #a9a9b9;
		line-height: 1.3;
		max-width: 36ch;
	}
</style>
