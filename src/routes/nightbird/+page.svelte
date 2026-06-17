<title>Nightbird Engine | Lycia Stenson</title>

<div class="space-y-5">
	<h1 class="text-5xl font-bold">
		Nightbird Engine
	</h1>

	<img src="/nightbird/editor.png" width="600" alt="Nightbird Editor" />

	<p class="text-lg">
		<a href="https://nightbirdlabs.github.io/engine" target="_blank" class="underline underline-offset-2 hover:text-violet-600 dark:hover:text-violet-300 transition-colors">
			Nightbird
		</a>
		is my cross-platform C++ game engine with Vulkan rendering on Windows and Linux, alongside Wii U and 3DS support.
	</p>

	<a
		class="flex px-2 space-x-2 items-center w-fit border-2 border-black dark:border-stone-400 text-black dark:text-white rounded-lg hover:shadow-lg duration-100 hover:scale-105"
		href="https://github.com/nightbirdlabs/Nightbird"
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
		After building an initial OpenGL renderer, I migrated to Vulkan to gain a deeper understanding of modern graphics pipelines. OpenGL abstracts a lot of what is really going on, and Vulkan felt like the natural progression as the modern open standard. I later abstracted platform-specifics behind backend interfaces allowing for Wii U and 3DS support. I wanted to challenge myself to get 3D rendering working on platforms significantly more constrained in processing and memory than modern PCs, so I chose my childhood consoles which have good homebrew support through devkitPro.
	</p>

	<p class="text-lg">
		On the desktop, a user&apos;s project can be compiled as a shared library loaded by the editor at runtime, or as a standalone executable. For Wii U and 3DS, the project is always compiled statically.
	</p>

	<h2 class="text-4xl font-bold">
		Reflection
	</h2>
	<p class="text-lg">
		Initially the editor used RTTR, an existing C++ reflection library, but it was unsuitable for the app since it relied on RTTI. This was especially the case on platforms like the Nintendo 3DS. Rather than maintain two separate reflection systems, I replaced RTTR entirely with a custom unified system that handles both field editing in the editor and binary scene loading in the app. This system handles type registration, field inspection via memory offsets, FNV hash-based type lookup, and runtime object instantiation.
	</p>

	<h2 class="text-4xl font-bold">
		Editor
	</h2>
	<div class="space-y-1">
		<p class="text-lg">
			The Nightbird Editor uses
			<a href="https://github.com/ocornut/imgui" class="italic">
				Dear ImGui
			</a>
			for its UI with the following windows:
		</p>
		<ul class="list-disc pl-8 space-y-1 text-lg">
			<li>Scene Outliner: Displays the objects in the scene in a reparentable hierarchy.</li>
			<li>Inspector: Displays editable serialised fields of the selected object or asset.</li>
			<li>Asset Browser: Browse folders and files within the Assets folder. Double-click on a scene to open it.</li>
			<li>Scene: Render and traverse the 3D scene from the perspective of the editor camera.</li>
		</ul>
	</div>

	<h2 class="text-4xl font-bold">
		Asset Cooking
	</h2>
	<p class="text-lg">
		Nightbird uses a two-stage pipeline for all assets. Scenes are saved by the editor as .ntscene files &lpar;Nightbird Text, TOML&rpar;, then cooked into .nbscene &lpar;Nightbird Binary&rpar; for runtime. Other assets are imported from source formats &lpar;.glb for meshes, .hdr for cubemaps, .flac and .wav for audio&rpar; and cooked into binary container formats &lpar;.nbmesh, .nbmaterial, .nbtexture, .nbaudio&rpar;.
	</p>
	<p class="text-lg">
		Cooking is platform-aware. On desktop, textures are currently stored as raw RGBA and audio as PCM. On Wii U, assets are byte-swapped at cook time, keeping load times down on the target platform. On 3DS, textures and audio are cooked into platform-native formats using tex3ds and VGAudioCli. Compressed format support for desktop and Wii U is planned.
	</p>

	<h2 class="text-4xl font-bold">
		Platforms
	</h2>
	<div class="space-y-1">
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
				</a>
				<ul class="list-disc pl-8 space-y-1 text-lg">
					<li>
						Tested in the
						<a href="https://cemu.info/" target="_blank" class="italic">
							Cemu
						</a> emulator
					</li>
				</ul>
			</li>
			<li>
				Nintendo 3DS - devkitPro
				<a href="https://github.com/devkitPro/libctru" target="_blank" class="italic">
					&lpar;libctru&rpar;
				</a>,
				<a href="https://github.com/devkitPro/citro3d" target="_blank" class="italic">
					&lpar;citro3d&rpar;
				</a>
				<ul class="list-disc pl-8 space-y-1 text-lg">
					<li>
						Tested on real hardware and in the
						<a href="https://azahar-emu.org/" target="_blank" class="italic">
							Azahar
						</a> emulator
					</li>
				</ul>
			</li>
		</ul>
	</div>
</div>
