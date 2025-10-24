<script>
	import ProjectCard from "$lib/components/ProjectCard.svelte";
</script>

<title>Lycia Stenson | Game Programmer</title>

<div class="space-y-6 p-8 text-black dark:text-white">
	<div class="space-y-4">
		<p class="text-xl">
			Hi, I'm a graduate game programmer focused on gameplay, graphics, and engine programming. Enjoys investigating problems and developing efficient solutions that improve designers&apos; workflows, with experience in Unreal, Unity, and Godot, and currently building a custom engine in C++ with Vulkan.
		</p>
		<p class="text-xl">
			Take a look at my favourite projects below.
		</p>
	</div>
	
	<h1 class="text-3xl font-bold">
		My Gameplay Programming Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-6">
		<ProjectCard title="Dance Brawler" description="A rhythm game disguised as a fighting game." details="As the gameplay programmer on the team, my primary responsiblity was to develop the note system." link="/dance-brawler"></ProjectCard>
		<ProjectCard title="Crimson Dust" description="Volunteer game project with a multidisciplinary team of designers and artists." details="Wild west themed game with fast-paced fighting built in Unreal." link="/crimson-dust"></ProjectCard>
		<ProjectCard title="3D Platformer" description="Super Mario 3D World-inspired 3D platformer." details="Created as a game feel demo to showcase the effects of movement and visual parameters." link="/3d-platformer"></ProjectCard>
		<ProjectCard title="LIDAR" description="The player fires rays which create dots when hitting the invisible environment." details="Rays are scattered throughout a cone shape with a radius that can be increased and decreased." link="/lidar"></ProjectCard>
		<ProjectCard title="Doctor Who" description="." details="These include a Mario-like 3D platformer and a Doctor Who-inspired demo with Weeping Angels and a TARDIS." link="/doctor-who"></ProjectCard>
	</div>
	
	<h1 class="text-3xl font-bold">
		My Engine and Graphics Programming Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-6">
		<ProjectCard title="Nightbird Engine" description="A custom game engine with Vulkan rendering." details="The engine includes 3D rendering with Vulkan, and an editor which can be used to browse assets, save and load scenes, and create and orient objects in the scene." link="/nightbird"></ProjectCard>
		<ProjectCard title="Witch Treehouse" description="A shader diorama written in C++ with OpenGL." details="Features shadow mapping and a Blinn-Phong lighting model." link="/witch-treehouse"></ProjectCard>
		<ProjectCard title="Dance Brawler" description="A rhythm game disguised as a fighting game." details="As the gameplay programmer on the team, my primary responsiblity was to develop the note system." link="/dance-brawler"></ProjectCard>
		<ProjectCard title="Godot Gameplay Prototypes" description="Various gameplay demos developed in Godot." details="These include a Mario-like 3D platformer and a Doctor Who-inspired demo with Weeping Angels and a TARDIS." link="/gameplay-prototypes"></ProjectCard>
	</div>
	
	<h1 class="text-3xl font-bold">
		My Other Projects
	</h1>
	
	<div class="flex flex-wrap justify-center gap-6">
		<ProjectCard title="Portfolio Website" description="Having some past experience with NextJS, I decided to build my portfolio website using SvelteKit." details="While my focus and passion is game development, I like to branch out into other areas of programming too." link="/"></ProjectCard>
		<ProjectCard title="Nightbird Website" description="I built the website for Nightbird Engine." details="Also using SvelteKit, the Nightbird website allowed me to develop skills designing websites with a modern appearance." link="https://nightbirdengine.github.io/"></ProjectCard>
	</div>
</div>