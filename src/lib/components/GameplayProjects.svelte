<script lang="ts">
	import ProjectCard from "./ProjectCard.svelte";
</script>

<h1 class="text-3xl font-bold">
	My Gameplay Programming Projects
</h1>

<div class="flex flex-wrap justify-center gap-4">
	<ProjectCard title="Dance Brawler" description="A rhythm game disguised as a fighting game." backgroundImage="/dance-brawler/thumbnail.jpg" logos={["/logos/unity.svg", "/logos/csharp.svg"]} link="/dance-brawler" />
	<ProjectCard title="Crimson Dust" description="Volunteer game project with a multidisciplinary team of designers and artists." backgroundImage="/crimson-dust/thumbnail.jpg" logos={["/logos/unreal.svg", "/logos/cpp.svg"]} link="/crimson-dust" />
	<ProjectCard title="Game Feel Demo" description="Super Mario-inspired platformer." backgroundImage="/game-feel-demo/thumbnail.jpg" logos={["/logos/godot.svg"]} link="/game-feel-demo" />
	<ProjectCard title="Doctor Who" description="Doctor Who demos featuring a &apos;Weeping Angel&apos; and a bigger-on-the-inside TARDIS." backgroundImage="/doctor-who/thumbnail.jpg" logos={["/logos/godot.svg", "logos/csharp.svg"]} link="/doctor-who" />
</div>