<script>
	import ProjectCard from "$lib/components/ProjectCard.svelte";
</script>

<title>Lycia Stenson | Game Programmer</title>

<div class="pt-4 p-8 text-black dark:text-white">
	<h1 class="pb-6 text-3xl font-bold">
		My Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-6">
		<ProjectCard title="Nightbird Engine" description="A custom game engine with Vulkan rendering." details="I started this project as an OpenGL renderer to develop my understanding of graphics programming. Nightbird grew into a bit of a game engine before migrating to Vulkan and further developing its capabilities such as a scene editor." link="/nightbird"></ProjectCard>
		<ProjectCard title="Witch Treehouse Diorama" description="A shader diorama featuring shadow mapping and a Blinn-Phong lighting model." details="Developed for a shaders assignment typically utilising an existing engine, I chose to take the opportunity to continue to develop Nightbird, which at the time was still an OpenGL renderer." link="/witch-treehouse"></ProjectCard>
		<ProjectCard title="Dance Brawler" description="A rhythm game disguised as a fighting game." details="As the gameplay programmer on the team, my primary responsiblity was to develop the note system." link="/dance-brawler"></ProjectCard>
	</div>
</div>