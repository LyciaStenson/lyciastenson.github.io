<script lang="ts">
	import CategoryCard from "$lib/components/CategoryCard.svelte";
	import ProjectCard from "$lib/components/ProjectCard.svelte";
	import GameplayProjects from "$lib/components/GameplayProjects.svelte";
	import EngineProjects from "$lib/components/EngineProjects.svelte";
</script>

<title>Lycia Stenson | Game Programmer</title>

<div class="space-y-6 text-black dark:text-white">
	<div class="space-y-4">
		<p class="text-xl">
			Hi, I'm a graduate game programmer focused on gameplay, graphics, and engine programming. I enjoy investigating problems and developing efficient solutions that improve designers&apos; workflows. I have experience in Unreal, Unity, and Godot, and I'm currently building a custom engine in C++ with Vulkan.
		</p>
	</div>
	
	<div class="flex flex-wrap justify-center gap-3 sm:gap-4 md:gap-6">
		<CategoryCard title="Gameplay Programming" link="/gameplay-programming" />
		<CategoryCard title="Engine &amp; Graphics Programming" link="/engine-programming" />
	</div>

	<GameplayProjects />
	<EngineProjects />
	
	<h1 class="text-3xl font-bold">
		My Other Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-4">
		<ProjectCard title="Web Development" description="Having some past experience with NextJS, I decided to build my portfolio and the Nightbird website using SvelteKit." backgroundImage="/web-development/thumbnail.jpg" blur={true} logos={["/logos/sveltekit.svg"]} link="/web-development" />
	</div>
</div>
