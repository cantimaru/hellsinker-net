<script>
	const tracks = [
		{ track: "TR_00", fanTitle: "THE GRAVEYARD", desc: "Title theme." },
		{ track: "TR_01", fanTitle: "EDGE OF THE GARDEN", desc: "SEGMENT 1 BEHIND" },
		{ track: "TR_02", fanTitle: "AN AWESOME PRAYER", desc: "General Boss Theme" },
		{ track: "TR_03", fanTitle: "OFF THE GULF OF SECT", desc: "SEGMENT 2 BEHIND" },
		{ track: "TR_04", fanTitle: "OPPOSITE OF THE VEIL", desc: "SEGMENT 3 BEHIND" },
		{ track: "TR_05", fanTitle: "SECRET PASSAGE", desc: "SEGMENT 4" },
		{ track: "TR_06", fanTitle: "RUSTED DRAGON", desc: "Rusted Dragon Boss Theme" },
		{ track: "TR_07", fanTitle: "DRIVING FACTOR", desc: "2nd title theme." },
		{ track: "TR_08", fanTitle: "DECIDE DESTINATION", desc: "Choosing between LEAD or BEHIND." },
		{ track: "TR_09", fanTitle: "ENTERING TO GARDEN", desc: "SEGMENT 1 LEAD" },
		{ track: "TR_10", fanTitle: "UNBREAKABLE CHAIN", desc: "SEGMENT 2 LEAD" },
		{ track: "TR_11", fanTitle: "SCARLET QUEEN", desc: "Secret form of the Scarlet Queen fight." },
		{ track: "TR_12", fanTitle: "INVISIBLE CRACKS", desc: "SEGMENT 3 LEAD" },
		{ track: "TR_13", fanTitle: "WATCHING THE STARS", desc: "Intermission theme." },
		{ track: "TR_14", fanTitle: "ON THE MEDALLION", desc: "SEGMENT 5 - SOL Side" },
		{ track: "TR_15", fanTitle: "ENIGMATIC UTERUS", desc: "SEGMENT 5 - LUNA Side" },
		{ track: "TR_16", fanTitle: "PERPETUAL CALENDAR", desc: "Perpetual Calendar Boss Theme, Sol side." },
		{ track: "TR_17", fanTitle: "THE GREAT CLOCK", desc: "Perpetual Calendar Boss Theme, Luna side." },
		{ track: "TR_18", fanTitle: "INTO CARDINAL", desc: "SEGMENT 6's introduction." },
		{ track: "TR_19", fanTitle: "CAVITIES OF DELUSION", desc: "SEGMENT 6's theme." },
		{ track: "TR_20-21", fanTitle: "PAST RISINGS AGAIN", desc: "Dawn and Dusk's / Apostles of the Seed boss theme. Actually a remix of Radio Zonde's boss music." },
		{ track: "TR_22", fanTitle: "MASTERLESS AND LOST", desc: "Entirety of SEGMENT 7's theme." },
		{ track: "TR_23", fanTitle: "We are Prayer.", desc: "Bad ending theme." },
		{ track: "TR_24", fanTitle: "SHRINE OF FAREWELL", desc: "Mausoleum" },
		{ track: "TR_25", fanTitle: "DESTINATION", desc: "SEGMENT 8 intermission." },
		{ track: "TR_26", fanTitle: "LAST DAWN WILL COME", desc: "SEGMENT 8's introduction." },
		{ track: "TR_27", fanTitle: "Even if this body feels no sun.", desc: "SEGMENT 8's theme, and the 3rd title theme." },
		{ track: "TR_28-29", fanTitle: "FATAL ATTRACTION", desc: "The Fatal Attraction be described as Hellsinker..." },
		{ track: "TR_30", fanTitle: "KAREIDOSCOPE", desc: "Last Boss I" },
		{ track: "TR_31", fanTitle: "PARADISE", desc: "Ending I" },
		{ track: "TR_32", fanTitle: "FLOCCINAUCINIHILIPILIFICATION", desc: "Last Boss II" },
		{ track: "TR_33", fanTitle: "<<VICTORY>>", desc: "Ending II" },
		{ track: "TR_34", fanTitle: "Brief Honeymoon", desc: "Name Entry" },
		{ track: "TR_35", fanTitle: "GARLAND", desc: "Last Boss III" },
		{ track: "TR_36", fanTitle: "LOST PROPERTY 771", desc: "True Finale" },
		{ track: "TR_37", fanTitle: "A Thing Left Behind", desc: "Name Entry, Full Clear" },
		{ track: "TR_38", fanTitle: "MEMENTO", desc: "4th title theme." },
		{ track: "TR_39", fanTitle: "THE GREAT MAJORITY", desc: "Extra Stage." },
		{ track: "TR_40", fanTitle: "THE WAY OF ALL FLESH", desc: "Second Extra Stage." },
		{ track: "TR_41", fanTitle: "THE AFTERIMAGE", desc: "Extra Intermission." },
		{ track: "TR_42", fanTitle: "ON THE EDGE OF CIRCLE", desc: "Ending Intermission." },
		{ track: "TR_43", fanTitle: "It's Absolutely.", desc: "Game over, man, game over!" },
		{ track: "TR_44", fanTitle: "A NOISY TEAPOT", desc: "Originally a seperate track on TONNOR's SoundCloud of which an older variation exists." },
		{ track: "TR_45", fanTitle: "EXPERIMENTAL CHAMBER", desc: "Originally a seperate track on TONNOR's SoundCloud of which an older variation exists." },
		{ track: "p_c_3a", fanTitle: "Knows Only Blazing", desc: "Song from TONNOR's SoundCloud. Interestingly, it has the motif of TR_12, but did not make it into the game. I like to imagine its use for a boss rush..." }
	];
</script>

<main>
	<h1>Music Tracks</h1>
	
	<p>A listing of all the music belonging to Hellsinker's original soundtrack. Unintuitively, the tracks were simply named TR_XX in order, so given names by Nautichor are provided for you to agree or disagree with.</p>

	<div class="grid">
		{#each tracks as track}
			{@const bgUrl = `url('/static/img/${track.track}.png')`}
			<article
				class="track-panel"
				style="--bg-image: {bgUrl}"
			>
				<h2 class="trackid">{track.track}</h2>
				<h4 class="fan-title">{track.fanTitle}</h4>

				<p class="track-desc">
					{track.desc || "Description goes here."}
				</p>
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
		background-image: linear-gradient(to bottom, #00000000, #000000FF), var(--bg-image);
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