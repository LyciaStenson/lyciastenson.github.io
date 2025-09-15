<script>
	import ProjectCard from "$lib/components/ProjectCard.svelte";
</script>

<title>Lycia Stenson | Game Programmer</title>

<div class="space-y-6 p-8 text-black dark:text-white">
	<p class="text-xl">
		Hi, I'm a graduate game programmer with an interest in gameplay and graphics programming. I love investigating problems and finding solutions to them.
	</p>
	<h1 class="pb-6 text-3xl font-bold">
		My Game Programming Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-6">
		<ProjectCard title="Nightbird Engine" description="A custom game engine with Vulkan rendering." details="I started this project as an OpenGL renderer to develop my understanding of graphics programming. Nightbird grew into a bit of a game engine before migrating to Vulkan and further developing its capabilities such as a scene editor." link="/nightbird"></ProjectCard>
		<ProjectCard title="Witch Treehouse Diorama" description="A shader diorama featuring shadow mapping and a Blinn-Phong lighting model." details="Developed for a shaders assignment typically utilising an existing engine, I chose to take the opportunity to continue to develop Nightbird, which at the time was still an OpenGL renderer." link="/witch-treehouse"></ProjectCard>
		<ProjectCard title="Dance Brawler" description="A rhythm game disguised as a fighting game." details="As the gameplay programmer on the team, my primary responsiblity was to develop the note system." link="/dance-brawler"></ProjectCard>
		<ProjectCard title="Boid Flocking" description="A boid flocking simulation developed in Unreal Engine." details="I used C++ with Unreal Engine to develop the simulation. I utilised Unreal's Instanced Static Mesh Component to increase performance with hundreds of boids." link="/boid-flocking"></ProjectCard>
		<ProjectCard title="3D Platformer" description="A 3D Mario-like platformer." details="A 3D platformer inspired by Super Mario 3D World, developed in Godot as a showcase of game feel for a university taster session." link="/3d-platformer"></ProjectCard>
	</div>

	<h1 class="pb-6 text-3xl font-bold">
		My Other Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-6">
		<ProjectCard title="Portfolio Website" description="Using some past experience with NextJS, I decided to build my portfolio website using SvelteKit." details="While my focus and passion is game development, I like to branch out into other areas of programming too." link="/"></ProjectCard>
	</div>
</div>