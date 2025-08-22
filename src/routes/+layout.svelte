<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<div class="flex flex-col min-h-screen">
	<header class="border-b-2 border-gray-400 p-4">
		<h1>Lycia Stenson | Game Programmer</h1>
	</header>
	
	<main class="flex-1">
		{@render children()}
	</main>
	
	<footer class="border-t-2 border-gray-400 text-center p-4">
		<h1>&copy; Lycia Stenson 2025</h1>
	</footer>
</div>
