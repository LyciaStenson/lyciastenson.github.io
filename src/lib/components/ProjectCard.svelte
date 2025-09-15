<script>
	export let title;
	export let description;
	export let details;
	export let link;
</script>

<a
	class="flex flex-col space-y-4 p-6 w-80 border-2 border-black dark:border-stone-400 text-black dark:text-white rounded-lg transition-transform duration-200 transform hover:scale-103"
	href={link}
>
	<h2 class="text-3xl font-semibold">{title}</h2>
	<div class="space-y-4">
		<p class="text-lg">
			{description}
		</p>
		<p class="text-md">
			{details}
		</p>
	</div>
</a>