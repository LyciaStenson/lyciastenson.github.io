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
	
	<img src="/nightbird/editor.png" width="600" alt="Portal issue" />
	
	<div class="space-y-2">
		<h2 class="text-4xl font-bold">
			Project System
		</h2>
		
		<div class="space-y-1">
			<p class="text-lg">
				Nightbird uses a shared library project system. The user's project code including custom object types are compiled as a DLL which is then loaded at runtime by the editor or app. Custom scene objects are listed along with built-in types in the editor with custom functionality when added to the scene.
			</p>
			
			<p class="text-lg">
				This is implemented using RTTR &lpar;Run Time Type Reflection&rpar; using the library&apos;s macros for users to register their types.
			</p>
		</div>
	</div>
	
	<div class="space-y-2">
		<h2 class="text-4xl font-bold">
			Scene
		</h2>
		
		<div class="space-y-1">
			<p class="text-lg">
				Scenes created in the editor can be saved and loaded in the game.
			</p>
		</div>
	</div>
	
	<div class="space-y-2">
		<h2 class="text-4xl font-bold">
			Vulkan Renderer
		</h2>
		
		<div class="space-y-1">
			<p class="text-lg">
				Nightbird uses a forward renderer implemented with Vulkan supporting opaque and transparent materials.
			</p>
			
			<p class="text-lg">
				Planned features include deferred rendering and PBR based on the Disney Principled BRDF.
			</p>
		</div>
	</div>
</div>