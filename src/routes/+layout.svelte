<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<style>
	@keyframes pulse-strong {
		0%, 100% {
			opacity: 0.05;
		}
		50% {
			opacity: 0.1;
		}
	}
	.animate-pulse-strong {
		animation: pulse-strong 5s ease-in-out infinite;
	}
</style>

<div class="fixed inset-0 -z-10 overflow-hidden pointer-events-none">
	<div
		class="absolute w-[60vw] h-[60vw] bg-linear-to-r from-purple-900 via-pink-600 to-purple-700 rounded-full blur-3xl animate-pulse-strong"
		style="top: 10%; left: 20%;">
	</div>
</div>

<div class="flex flex-col min-h-screen text-black dark:text-white">
	<header class="sticky top-0 z-50 text-lg p-6 border-b-2 border-stone-400 bg-white dark:bg-stone-950">
		<h1>
			<a href="/">
				Lycia Stenson | Game Programmer
			</a>
		</h1>
	</header>
	
	<main class="flex-1 p-4 sm:p-8 md:px-14 md:py-14 max-w-360 mx-auto">
		{@render children()}
	</main>
	
	<footer class="border-t-2 border-stone-400 text-center p-4">
		<h1>&copy; 2025 Lycia Stenson</h1>
	</footer>
</div>
