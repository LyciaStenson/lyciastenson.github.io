<script lang="ts">
	export let title: string;
	export let description: string;
	export let backgroundImage: string | null = null;
	export let blur: boolean = false;
	export let logos: string[] = [];
	export let link: string;
</script>

<a
	class="group relative overflow-hidden flex flex-col justify-end p-2 w-full md:w-80 min-h-98 border-2 border-black dark:border-stone-400 text-black dark:text-white rounded-lg hover:shadow-lg"
	href={link}
>
	<div
		class="absolute inset-0 bg-cover bg-center duration-200 group-hover:scale-110 filter {blur ? 'blur-sm' : ''}"
		style="background-image: {backgroundImage ? `url(${backgroundImage})` : 'none'}"
	></div>
	
	<div class="absolute inset-0 bg-black/15 dark:bg-black/30 transition-opacity duration-50 group-hover:opacity-0"></div>

	{#if logos.length > 0}
	<div class="absolute top-2 left-2 flex gap-2 z-20 p-1 rounded-md bg-white/65 dark:bg-black/65">
		{#each logos as logo}
		<img src={logo} alt="Logo" class="h-7 dark:invert" />
		{/each}
	</div>
	{/if}
	
	<div class="relative pointer-events-none hover-a z-10 space-y-1 p-2 rounded-md bg-white/65 dark:bg-black/65">
		<h2 class="text-3xl font-semibold">{title}</h2>
		
		<p class="text-md">
			{description}
		</p>
	</div>
</a>