<script lang="ts">
	let games = $state([
		{
			name: "Tobarinker // とばりんかー",
			developer: "Trickster Jam",
			release: "2010-09-30",
			desc: "N/A",
		},
		{
			name: "Shaftdiver",
			developer: "D.N.A. Softwares",
			release: "2010-08-09",
			desc: "N/A",
		},
		{
			name: "PUZZSINKER.",
			developer: "CAT'S WHISPER",
			release: "2010-06-07",
			desc: "N/A",
		},
		{
			name: "シンカノゲーム",
			developer: "OMEGA",
			release: "2010-07-04",
			desc: "N/A",
		},
	]);

	let doujinshi = $state([
		{ name: "TARGETマッシグラ", author: "TARGETマッシグラ製作委員会", release: "2007-11-03", desc: "N/A" },
		{ name: "STGGER：ONE", author: "trickster.jam", release: "2007-12-31", desc: "N/A" },
		{ name: "MINOSINKER． EX", author: "7－iro", release: "2008-08-16", desc: "N/A" },
		{ name: "TARGETマッシグラ Seg.2", author: "TARGETマッシグラ製作委員会", release: "2008-08-16", desc: "N/A" },
		{ name: "MINOSINKER. 霊廟", author: "7－iro", release: "2008-11-03", desc: "N/A" },
		{ name: "みのがめたっぷり 01", author: "にゃんぷに会", release: "2008-11-03", desc: "N/A" },
		{ name: "プレイビョ～イ", author: "Nyanpuni-kai", release: "2008-12-29", desc: "N/A" },
		{ name: "へ漫ら", author: "SYS-LILA", release: "2009-06-07", desc: "N/A" },
		{ name: "めいでんたっぷり 02", author: "にゃんぷに会", release: "2009-06-07", desc: "N/A" },
		{ name: "翔び出せグレイブヤード", author: "IMPERIAL CROWN/クラムボンの微笑", release: "2009-06-07", desc: "N/A" },
		{ name: "巨大ロボKAGURA みっつの勇気が一つになればちりじんむ(笑)", author: "簡易溶接所", release: "2009-06-07", desc: "N/A" },
		{ name: "RZ×HS", author: "trickster.jam", release: "2009-08-15", desc: "N/A" },
		{ name: "花冠一年生 8月号", author: "Nyanpuni-kai", release: "2009-08-15", desc: "N/A" },
		{ name: "この鯖竜がお買い得。", author: "鶏肉生活", release: "2009-08-15", desc: "N/A" },
		{ name: "みのしんかー 後光 MINOSINKER", author: "7－iro", release: "2009-08-15", desc: "N/A" },
		{ name: "あきひろたっぷり 03", author: "にゃんぷに会", release: "2009-12-30", desc: "N/A" },
		{ name: "A THING RIGHT BEHIND", author: "Aylove.org", release: "2010-07-04", desc: "N/A" },
		{ name: "ボリューム満点!!犬丼定食", author: "Nyanpuni-kai", release: "2010-07-04", desc: "N/A" },
		{ name: "へるしんカレー", author: "シヱスタリア", release: "2010-07-04", desc: "N/A" },
		{ name: "ABYSS RISER", author: "残酷綿棒", release: "2010-07-04", desc: "N/A" },
		{ name: "THORNED CHAIN AND MEMENTO MESSAGE", author: "AILI", release: "2010-07-04", desc: "N/A" },
		{ name: "みのニー", author: "SYS-LILA", release: "2010-07-04", desc: "N/A" },
		{ name: "ぺどしんか", author: "にゃんぷに会", release: "2010-08-15", desc: "N/A" },
		{ name: "すぐりんか", author: "7－iro", release: "2011-12-31", desc: "N/A" },
		{ name: "プレイヤーズ", author: "ちょこびゐる", release: "2012-08-11", desc: "N/A" },
		{ name: "みのしんかーKYD", author: "7－iro", release: "2013-12-31", desc: "N/A" },
		{ name: "はだいろたっぷり 2", author: "にゃんぷに会", release: "UNKNOWN", desc: "N/A" },
		{ name: "MINOSINKER.", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: "MINOSINKER. 花冠", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: "MINOSINKER☆", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: "MINOSINKER 後光", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: "みのしんかー　英霊", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: "みのしんかー７７１", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: "みのしんかー９，０００，０００", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: " みのしんかー概要と手引き", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: "すかいみのちゃん", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
		{ name: "みのしんかーQUASAR", author: "7－iro", release: "UNKNOWN", desc: "N/A" },
	]);

	let albums = $state([
		{ name: "Without reStraint", artist: "Sound Ave.", release: "2007-12-31", desc: "N/A" },
		{ name: "DiGITALiZM -デジタリズム-", artist: "MARS Tracks", release: "2007-12-31", desc: "N/A" },
		{ name: "AUDIENCE WITH PRAYER", artist: "Machia Works", release: "2007-12-31", desc: "N/A" },
	]);
</script>

<!-- TODO: Archive tables should be expandable with a brief explanation up on top and maybe some describtiopons for each of the gings okay Bye -->

<h1>Fanworks Archive</h1>
<hr/>

<h2>Games</h2>
<table>
	<thead>
		<tr>
			<th>Title</th>
			<th>Developer</th>
			<th>Release Date</th>
			<th>Info</th>
		</tr>
	</thead>
	<tbody>
		{#each games as game}
			<tr>
				<td>{game.name}</td>
				<td>{game.developer}</td>
				<td>{game.release}</td>
				<td>{game.desc}</td>
			</tr>
		{/each}
	</tbody>
</table>

<!-- <h3></h3>

<h3></h3>

<h3></h3> -->

<h2>Doujinshi</h2>

<table>
	<thead>
		<tr>
			<th>Title</th>
			<th>Developer</th>
			<th>Release Date</th>
			<th>Info</th>
		</tr>
	</thead>
	<tbody>
		{#each doujinshi as doujin}
			<tr>
				<td>{doujin.name}</td>
				<td>{doujin.author}</td>
				<td>{doujin.release}</td>
				<td>{doujin.desc}</td>
			</tr>
		{/each}
	</tbody>
</table>

<h2>Music</h2>

<table>
	<thead>
		<tr>
			<th>Title</th>
			<th>Developer</th>
			<th>Release Date</th>
			<th>Info</th>
		</tr>
	</thead>
	<tbody>
		{#each albums as album}
			<tr>
				<td>{album.name}</td>
				<td>{album.artist}</td>
				<td>{album.release}</td>
				<td>{album.desc}</td>
			</tr>
		{/each}
	</tbody>
</table>