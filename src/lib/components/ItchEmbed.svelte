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

<iframe title="Itch Embed" height="167" frameborder="0" src={iframeSrc} width="552">
</iframe>