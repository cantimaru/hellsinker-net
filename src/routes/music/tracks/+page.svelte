<script>
	import TrackGrid from '$lib/tracks.svelte'

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

	<TrackGrid {tracks} />
	

	<p>
		<small
			>It's rather interesting how SEGMENT 2 BEHIND's theme is the
			most-referenced despite the low percieved significance of that
			stage.</small
		>
	</p>

	<hr />
</main>