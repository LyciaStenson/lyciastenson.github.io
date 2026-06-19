<script lang="ts">
	import ProjectCard from "./ProjectCard.svelte";
</script>

<h1 class="text-3xl font-bold">
	My Engine &amp; Graphics Programming Projects
</h1>

<div class="flex flex-wrap justify-center gap-4">
	<ProjectCard title="Nightbird Engine" description="Cross-platform C++ game engine with desktop Vulkan rendering, alongside Wii U and 3DS support" backgroundImage="/nightbird/thumbnail.jpg" logos={["/logos/cpp.svg", "/logos/vulkan.svg"]} link="/nightbird" />
	<ProjectCard title="Witch Treehouse" description="A shader diorama written in C++ with OpenGL." backgroundImage="/witch-treehouse/thumbnail.jpg" logos={["/logos/cpp.svg", "/logos/opengl.svg"]} link="/witch-treehouse" />
	<ProjectCard title="LIDAR" description="The player fires rays which create dots when hitting the invisible environment." backgroundImage="/lidar/thumbnail.png" logos={["/logos/godot.svg"]} link="/lidar" />
</div>