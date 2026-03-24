<title>Nightbird Engine | Lycia Stenson</title>

<div class="space-y-5">
	<h1 class="text-5xl font-bold">
		Nightbird Engine
	</h1>
	
	<p class="text-lg">
		Nightbird is my cross-platform C++ game engine with Vulkan rendering, supporting Windows and Linux with potential future macOS support.
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
		Started as an OpenGL renderer to develop my understanding of graphics programming, the project became my own game engine. I migrated to Vulkan.
	</p>
	
	<img src="/nightbird/editor.png" width="600" alt="Nightbird Editor" />
	
	<div class="space-y-2">
		<h2 class="text-4xl font-bold">
			Cross-Platform
		</h2>
		
		<div class="space-y-1">
			<p class="text-lg">
				A backend system allows platform and rendering functionality to be implemented for different platforms.
			</p>
			<div class="space-y-0">
				<p class="text-lg font-semibold">
					Tested Environments:
				</p>
				<ul class="list-disc pl-8 space-y-1 text-lg">
					<li>
						Windows 10 &amp; 11 - Visual Studio 2022
						<a href="https://premake.github.io/" target="_blank" class="italic">
							&lpar;Premake&rpar;
						</a>
					</li>
					<li>
						Linux - Make &amp; GCC
						<a href="https://premake.github.io/" target="_blank" class="italic">
							&lpar;Premake&rpar;
						</a>
					</li>
					<li>
						Nintendo Wii U - devkitPro
						<a href="https://github.com/devkitPro/wut" target="_blank" class="italic">
							&lpar;wut&rpar;
						</a>,
						<a href="https://github.com/Exzap/CafeGLSL" target="_blank" class="italic">
							&lpar;CafeGLSL&rpar;
						</a>,
					</li>
					<li>
						Nintendo 3DS - devkitPro
						<a href="https://github.com/devkitPro/libctru" target="_blank" class="italic">
							&lpar;libctru&rpar;
						</a>,
						<a href="https://github.com/devkitPro/citro3d" target="_blank" class="italic">
							&lpar;citro3d&rpar;
						</a>
					</li>
				</ul>
			</div>
		</div>
	</div>
	
	<div class="space-y-2">
		<h2 class="text-4xl font-bold">
			Projects
		</h2>
		
		<div class="space-y-1">
			<p class="text-lg">
				Project code containing custom object types is compiled as a shared library and loaded at runtime. These types are displayed alongside built-in objects in the editor, with custom properties exposed in the inspector and custom behaviour during simulation.
			</p>
			
			<p class="text-lg">
				This is implemented using
				<a href="https://www.rttr.org/" class="font-semibold">
					RTTR &lpar;Run Time Type Reflection&rpar;
				</a>
				using the library&apos;s macros for users to register their types.
			</p>
		</div>
	</div>
	
	<div class="space-y-2">
		<h2 class="text-4xl font-bold">
			Scenes
		</h2>
		
		<div class="space-y-1">
			<p class="text-lg">
				Scenes created in the editor can be saved and loaded in the game.
			</p>
			<p class="text-lg">
				Models are serialised with only the path to the .glb file, and the hierarchy is recreated upon loading the scene.
			</p>
		</div>
	</div>

	<div class="space-y-2">
		<h2 class="text-4xl font-bold">
			App
		</h2>
		
		<div class="space-y-1">
			<p class="text-lg">
				The Nightbird App is the executable where simulation is enabled, and the scene is rendered from the scene's Main Camera directly to the swap chain framebuffer.
			</p>
		</div>
	</div>
	
	<div class="space-y-2">
		<h2 class="text-4xl font-bold">
			Editor
		</h2>
		
		<div class="space-y-1">
			<p class="text-lg">
				The Nightbird editor is implemented using
				<a href="https://github.com/ocornut/imgui" class="font-semibold">
					Dear ImGui.
				</a>
			</p>
			
			<div class="space-y-0">
				<p class="text-lg">
					The editor features various windows:
				</p>
				<ul class="list-disc pl-8 space-y-1 text-lg">
					<li>Scene Outliner - Displays the objects in the scene in a reparentable hierarchy</li>
					<li>Inspector - Displays serialised properties of the selected object</li>
					<li>Asset Browser - Browse folders and files contained within the Assets folder. Double-click on a scene to open it.</li>
					<li>Scene - Render and traverse the 3D scene from the perspective of the Editor Camera.</li>
				</ul>
				<p class="text-lg">
					A Game window is planned where the scene will be rendered from the main camera, as in the App.
				</p>
			</div>
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