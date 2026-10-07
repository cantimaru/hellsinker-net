<script>
    import TrackGrid from '$lib/tracks.svelte'

    const tracks = [
		{
			track: "TR_NULL",
			fanTitle: "NULLS ONLY BLAZING",
			desc: "NULLDESC",
			motifs: ["NULLTIFS"],
		},
	];
</script>

<main>
<h1>0.95 Tracks</h1>
    <TrackGrid {tracks} />
</main>