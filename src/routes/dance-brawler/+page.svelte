<script lang="ts">
	import ItchEmbed from "$lib/components/ItchEmbed.svelte";
</script>

<title>Dance Brawler | Lycia Stenson</title>

<div class="space-y-5">
	<h1 class="text-5xl font-bold">
		Dance Brawler
	</h1>
	
	<p class="text-lg">
		A rhythm game disguised as a fighting game. Inspired by Friday Night Funkin in gameplay and Street Fighter in aesthetic.
	</p>
	
	<div class="aspect-video max-w-2xl">
		<iframe
			class="w-full h-full"
			src="https://www.youtube.com/embed/RI026_hx8Tk"
			title="YouTube video player"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
			allowfullscreen
		></iframe>
	</div>
	
	<div class="space-y-1">
		<p class="text-lg">
			This was my final year group project at university. I worked in a team of 7 to develop the game in four months.
		</p>
		
		<p class="text-lg">
			As the gameplay programmer I built the note system, featuring various types of notes, and ensuring that the timing of player input and the visual representation of notes matched.
		</p>
	</div>
	
	<div class="space-y-1">
		<p class="text-lg">
			Note Types
		</p>
		<ul class="list-disc pl-8 space-y-1">
			<li>Single Note - Must be hit as it passes the hit area</li>
			<li>Hold Note - Has a duration where the button must be held</li>
			<li>Mash Note - Has a duration where the button must be pressed repeatedly</li>
			<li>Ghost Note - Fades out as it approaches the hit area</li>
			<li>Trick Note - Initially in the wrong lane before sliding into the correct lane as they approach the hit area</li>
			<li>Bomb Note - Must not be hit</li>
		</ul>
	</div>
	
	<p class="text-lg">
		I also built the Stance Change system, a gameplay mechanic where the inputs change throughout the song. This starts with D-Pad and changes to Face Buttons, Bumpes/Triggers, and finally all inputs.
	</p>
	
	<ItchEmbed gameId="3577174" />
</div>