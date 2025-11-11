<script lang="ts">
	import { onMount } from "svelte";
	import { browser } from "$app/environment";
	
	export let gameId: string;

	let isDark: boolean = false;

	if (browser) {
		onMount(() => {
			const mediaQuery: MediaQueryList = window.matchMedia('(prefers-color-scheme: dark)');
			isDark = mediaQuery.matches;
			
			const updateTheme = (e: MediaQueryListEvent) => {
				isDark = e.matches;
			};
			
			mediaQuery.addEventListener('change', updateTheme);
			
			return () => {
				mediaQuery.removeEventListener('change', updateTheme);
			};
		});
	}
	
	$: iframeSrc = `https://itch.io/embed/${gameId}${isDark ? '/?dark=true' : ''}`;
</script>

<div class="w-full max-w-[552px] h-[147px] sm:h-[167px]">
	<iframe
		title="Itch Embed"
		class="w-full h-full border-0"
		src={iframeSrc}
	>
	</iframe>
</div>