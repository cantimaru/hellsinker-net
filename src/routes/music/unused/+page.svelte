<script>
    import TrackGrid from '$lib/tracks.svelte'

    const tracks = [
		{
			track: "p_c_3a",
			fanTitle: "Knows Only Blazing",
			desc: "Song from TONNOR's SoundCloud that did not make it into the game. I like to imagine its use for a boss rush...",
			motifs: ["TR_01", "TR_09", "TR_12"],
		},
		{
			track: "bbt_pak-0000000001",
			desc: "An unused track that likely would have served as menu music.",
		},
		{
			track: "bbt_pak-0000000007",
			desc: "A short 9 second loop featuring chimes and chants, presumably related to the shrine.",
		},
		{
			track: "bbt_pak-000000009",
			desc: "An alternative mix of the track featured in extra stage 2, THE WAY OF ALL FLESH.",
		},
		{
			track: "bbt_pak-0000000011",
			desc: "A 1:20 minute track with howling winds and an ominous organ humming in the background, seemingly an unused credits track.",
		},
		{
			track: "bbt_pak-0000000018",
			desc: 'An alternative version of the "GAME OVER" track.',
		},
		{
			track: "bbt_pak-0000000022",
			desc: "",
		},
		{
			track: "bbt_pak-0000000030",
			desc: "An alternative variant of the TLB3 section 2 track, less complex and structured in its sound design, also tonally a lot more tame.",
		},
		{
			track: "bbt_pak-0000000033",
			desc: "Presumably a text intermission theme. Repetitive and acquainted by a choir, possibly a bad end track.",
		},
		{
			track: "bbt_pak-0000000037",
			desc: "Strong similarity to the track played in The Great Majority, much more calm and passive in design. Possibly a prototype.",
		},
		{
			track: "bbt_pak-0000000041",
			desc: "Freakishly jazzy, completely alien to the soundtrack that was and is. No clue how this would have fit in.",
		},
		{
			track: "bbt_pak-0000000052",
			desc: "A remixed version of Segment 4 from the 0.95 edition of Hellsinker.",
		},
		{
			track: "bbt_pak-0000000053",
			desc: "An alternative version of stage 5's SOL side, ON THE MEDALLION.",
		},
		{
			track: "bbt_pak-0000000055",
			desc: 'An alternative version of segment 7\'s, MASTERLESS AND LOST. The body is noticably different in its mixing, and the boss section feels a lot "lighter."',
		},
		{
			track: "bbt_pak-0000000057",
			desc: "An alternative version of segment 6's boss track, there's a very clear itwangi not previously present. The guitar is not as heavy here too.",
		},
		{
			track: "bbt_pak-0000000059",
			desc: "A prototype version of the stage select track, this one is half in length while also having a different body. It is also has quite much in common with bbt_pak-0...033",
		},
	];
</script>

<main>
<h1>Unused Tracks</h1>
    <TrackGrid {tracks} />
</main>