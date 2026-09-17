<script>
	const tracks = [
		{
			track: "TR_00",
			fanTitle: "THE GRAVEYARD",
			desc: "Title theme.",
		},
		{
			track: "TR_01",
			fanTitle: "EDGE OF THE GARDEN",
			desc: "SEGMENT 1 BEHIND",
		},
		{
			track: "TR_02",
			fanTitle: "AN AWESOME PRAYER",
			desc: "General Boss Theme",
		},
		{
			track: "TR_03",
			fanTitle: "OFF THE GULF OF SECT",
			desc: "SEGMENT 2 BEHIND",
		},
		{
			track: "TR_04",
			fanTitle: "OPPOSITE OF THE VEIL",
			desc: "SEGMENT 3 BEHIND",
			motifs: ["TR_02"],
		},
		{
			track: "TR_05",
			fanTitle: "SECRET PASSAGE",
			desc: "SEGMENT 4",
		},
		{
			track: "TR_06",
			fanTitle: "RUSTED DRAGON",
			desc: "Rusted Dragon Boss Theme",
		},
		{
			track: "TR_07",
			fanTitle: "DRIVING FACTOR",
			desc: "2nd title theme.",
		},
		{
			track: "TR_08",
			fanTitle: "DECIDE DESTINATION",
			desc: "Choosing between LEAD or BEHIND.",
		},
		{
			track: "TR_09",
			fanTitle: "ENTERING TO GARDEN",
			desc: "SEGMENT 1 LEAD",
			motifs: ["TR_01", "TR_07"],
		},
		{
			track: "TR_10",
			fanTitle: "UNBREAKABLE CHAIN",
			desc: "SEGMENT 2 LEAD",
		},
		{
			track: "TR_11",
			fanTitle: "SCARLET QUEEN",
			desc: "Secret form of the Scarlet Queen fight.",
			motifs: ["TR_02"],
		},
		{
			track: "TR_12",
			fanTitle: "INVISIBLE CRACKS",
			desc: "SEGMENT 3 LEAD",
		},
		{
			track: "TR_13",
			fanTitle: "WATCHING THE STARS",
			desc: "Intermission theme.",
		},
		{
			track: "TR_14",
			fanTitle: "ON THE MEDALLION",
			desc: "SEGMENT 5 - SOL Side",
		},
		{
			track: "TR_15",
			fanTitle: "ENIGMATIC UTERUS",
			desc: "SEGMENT 5 - LUNA Side",
			motifs: ["TR_14"],
		},
		{
			track: "TR_16",
			fanTitle: "PERPETUAL CALENDAR",
			desc: "Perpetual Calendar Boss Theme, Sol side.",
		},
		{
			track: "TR_17",
			fanTitle: "THE GREAT CLOCK",
			desc: "Perpetual Calendar Boss Theme, Luna side.",
			motifs: ["TR_16"],
		},
		{
			track: "TR_18",
			fanTitle: "INTO CARDINAL",
			desc: "SEGMENT 6's introduction.",
			motifs: ["TR_00"],
		},
		{
			track: "TR_19",
			fanTitle: "CAVITIES OF DELUSION",
			desc: "SEGMENT 6's theme.",
		},
		{
			track: "TR_20-21",
			fanTitle: "PAST RISINGS AGAIN",
			desc: "Dawn and Dusk's / Apostles of the Seed boss theme. Is, in fact, a remix of Radio Zonde's boss music.",
		},
		{
			track: "TR_22",
			fanTitle: "MASTERLESS AND LOST",
			desc: "Entirety of SEGMENT 7's theme.",
		},
		{
			track: "TR_23",
			fanTitle: "We are Prayer.",
			desc: "Bad ending theme.",
		},
		{
			track: "TR_24",
			fanTitle: "SHRINE OF FAREWELL",
			desc: "Mausoleum",
		},
		{
			track: "TR_25",
			fanTitle: "DESTINATION",
			desc: "SEGMENT 8 intermission.",
			motifs: ["TR_08"],
		},
		{
			track: "TR_26",
			fanTitle: "LAST DAWN WILL COME",
			desc: "SEGMENT 8's introduction.",
			motifs: ["TR_01"],
		},
		{
			track: "TR_27",
			fanTitle: "Even if this body feels no sun.",
			desc: "SEGMENT 8's theme, and the 3rd title theme.",
		},
		{
			track: "TR_28-29",
			fanTitle: "FATAL ATTRACTION",
			desc: "The Fatal Attraction be described as Hellsinker...",
		},
		{
			track: "TR_30",
			fanTitle: "KAREIDOSCOPE",
			desc: "Last Boss I",
			motifs: ["TR_01", "TR_09"],
		},
		{
			track: "TR_31",
			fanTitle: "PARADISE",
			desc: "Ending I",
		},
		{
			track: "TR_32",
			fanTitle: "FLOCCINAUCINIHILIPILIFICATION",
			desc: "Last Boss II",
			motifs: ["TR_03", "TR_23"],
		},
		{
			track: "TR_33",
			fanTitle: "<<VICTORY>>",
			desc: "Ending II",
			motifs: ["TR_03"],
		},
		{
			track: "TR_34",
			fanTitle: "Brief Honeymoon",
			desc: "Name Entry",
		},
		{
			track: "TR_35",
			fanTitle: "GARLAND",
			desc: "Last Boss III",
			motifs: ["TR_23"],
		},
		{
			track: "TR_36",
			fanTitle: "LOST PROPERTY 771",
			desc: "True Finale",
			motifs: ["TR_03"],
		},
		{
			track: "TR_37",
			fanTitle: "A Thing Left Behind",
			desc: "Name Entry, Full Clear",
			motifs: ["TR_34"],
		},
		{
			track: "TR_38",
			fanTitle: "MEMENTO",
			desc: "4th title theme.",
		},
		{
			track: "TR_39",
			fanTitle: "THE GREAT MAJORITY",
			desc: "Extra Stage.",
			motifs: ["TR_14", "TR_15"],
		},
		{
			track: "TR_40",
			fanTitle: "THE WAY OF ALL FLESH",
			desc: "Second Extra Stage.",
			motifs: ["TR_00", "TR_10", "TR_14", "TR_15", "TR_21", "TR_39"],
		},
		{
			track: "TR_41",
			fanTitle: "THE AFTERIMAGE",
			desc: "Intermission surrounding THE GREAT MAJORITY.",
		},
		{
			track: "TR_42",
			fanTitle: "ON THE EDGE OF CIRCLE",
			desc: "Ending Intermission after THE WAY OF ALL FLESH.",
		},
		{
			track: "TR_43",
			fanTitle: "It's Absolutely.",
			desc: "Game over, man, game over!",
		},
		{
			track: "TR_44",
			fanTitle: "A NOISY TEAPOT",
			desc: "Originally a seperate track on TONNOR's SoundCloud of which an older variation exists.",
			motifs: ["TR_00"],
		},
		{
			track: "TR_45",
			fanTitle: "EXPERIMENTAL CHAMBER",
			desc: "Originally a seperate track on TONNOR's SoundCloud of which an older variation exists.",
			motifs: ["TR_00"],
		},
	];

	const unusedtracks = [
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
	<h1>Music Tracks</h1>

	<p>
		A listing of all the music belonging to Hellsinker's original
		soundtrack. Unintuitively, the tracks were simply named TR_XX in order,
		so given names by Nautichor are provided for you to agree or disagree
		with. Additionally, tracks will list any leitmotifs (reoccuring
		melodies) - if any - heard in prior tracks <i>only</i>, due to the
		linear nature of the game and soundtrack.<br />
		<small
			>Someday, it'd be neat to find the sound sources for Hellsinker's
			OST.</small
		>
	</p>

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

	<p>
		<small
			>It's rather interesting how SEGMENT 2 BEHIND's theme is the
			most-referenced despite the low percieved significance of that
			stage.</small
		>
	</p>

	<hr />
	<h1>Unused Tracks</h1>

	<div class="grid">
		{#each unusedtracks as track}
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
</main>

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
