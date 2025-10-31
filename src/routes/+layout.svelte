<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<div class="flex flex-col min-h-screen bg-white dark:bg-stone-950 text-black dark:text-white">
	<header class="sticky top-0 z-50 text-lg p-6 border-b-2 border-stone-400 bg-white dark:bg-stone-950">
		<h1>
			<a href="/">
				Lycia Stenson | Game Programmer
			</a>
		</h1>
	</header>
	
	<main class="flex-1">
		<div class="p-4 sm:p-8 md:px-18 md:py-14 max-w-7xl mx-auto w-full">
			{@render children()}
		</div>
	</main>
	
	<footer class="border-t-2 border-stone-400 text-center p-4">
		<h1>&copy; 2025 Lycia Stenson</h1>
	</footer>
</div>
