<script>
	import ProjectCard from "$lib/components/ProjectCard.svelte";
</script>

<title>Lycia Stenson | Game Graphics Programmer</title>

<div class="pt-4 p-8">
	<h1 class="pb-6 text-3xl font-bold">
		My Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-6">
		<ProjectCard title="Nightbird" description="A custom game engine with OpenGL rendering." details="I started this project to develop my understanding of real-time graphics. Other students on my course joined the project, while my focus remains the graphics." link="https://nightbirdengine.github.io"></ProjectCard>
		<ProjectCard title="Witch Treehouse Diorama" description="A shader diorama featuring Nightbird's shadow mapping and Blinn-Phong lighting model" details="I chose to take the opportunity to continue to develop Nightbird, while the assignment expected the use of an existing graphics engine." link="https://nightbirdengine.github.io"></ProjectCard>
		<ProjectCard title="Graphics API Research" description="Why is the real-time graphics industry adopting low-level graphics APIs such as Vulkan over high-level APIs like OpenGL?" details="I am researching the adoption of low-level graphics APIs by the real-time graphics industry." link="https://lyciastenson.github.io"></ProjectCard>
		<ProjectCard title="Sublime" description="A custom offline ray traced renderer. Currently developing a command-line interface." details="In future a Blender add-on will be developed to render scenes." link="https://lyciastenson.github.io"></ProjectCard>
	</div>
</div>