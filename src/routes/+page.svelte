<script>
	import ProjectCard from "$lib/components/ProjectCard.svelte";
</script>

<title>Lycia Stenson | Game Programmer</title>

<div class="pt-4 p-8">
	<h1 class="pb-6 text-3xl font-bold">
		My Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-6">
		<ProjectCard title="Nightbird" description="A custom game engine with OpenGL rendering." details="I started this project to develop my understanding of real-time graphics. Other students on my course joined the project, while my focus remains the graphics." link="https://nightbirdengine.github.io"></ProjectCard>
		<ProjectCard title="Witch Treehouse Diorama" description="A shader diorama featuring shadow mapping and a Blinn-Phong lighting model." details="Developed for a shaders assignment typically utilising an existing engine, I chose to take the opportunity to continue to develop Nightbird." link="https://nightbirdengine.github.io"></ProjectCard>
		<ProjectCard title="Vulkan Renderer" description="A simple C++ Vulkan renderer" details="" link="https://nightbirdengine.github.io"></ProjectCard>
		<ProjectCard title="Dance Brawler" description="A rhythm game disguised as a fighting game." details="I worked as the gameplay programmer." link="https://dancebrawler.github.io"></ProjectCard>
	</div>
</div>