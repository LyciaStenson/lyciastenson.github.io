<title>Nightbird Engine | Lycia Stenson</title>

<div class="space-y-5">
	<h1 class="text-5xl font-bold">
		Nightbird Engine
	</h1>
	
	<p class="text-lg">
		Nightbird is my custom C++ game engine with Vulkan rendering.
	</p>
	
	<a
		class="flex px-2 space-x-2 items-center w-fit border-2 border-black dark:border-stone-400 text-black dark:text-white rounded-lg hover:shadow-lg duration-100 hover:scale-105"
		href="https://github.com/NightbirdEngine/Nightbird"
	>
		<img src="/logos/github-icon.svg" alt="GitHub Icon" class="h-10 dark:invert"/>
		<div class="pb-1.5">
			<p class="text-lg font-bold">
				Available on
			</p>
			<img src="/logos/github-text.svg" alt="GitHub Icon" class="h-6 dark:invert"/>
		</div>
	</a>
	
	<p class="text-lg">
		This project started as an OpenGL renderer to develop my understanding of graphics programming. The project developed into my own game engine. I migrated to Vulkan and further developed its capabilities such as the scene editor and project system.
	</p>
	
	<div class="space-y-1">
		<p class="text-lg">
			The engine features runtime type reflection and a dynamic project system using RTTR.
		</p>
		<p class="text-lg">
			The user's project code is compiled as a DLL which is loaded by the editor or game at runtime. Custom scene object classes are listed along with built-in types in the editor and can have custom functionality when added to the scene.
		</p>
		<p class="text-lg">
			Scenes created in the editor can be saved and loaded in the game.
		</p>
	</div>
	
	<img src="/nightbird/editor.png" width="600" alt="Portal issue" />
</div>