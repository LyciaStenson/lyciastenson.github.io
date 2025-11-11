<title>LIDAR | Lycia Stenson</title>

<div class="space-y-5">
	<h1 class="text-5xl font-bold">
		LIDAR
	</h1>
	
	<div class="space-y-3">
		<p class="text-lg">
			The player uses a &apos;LIDAR scanner&apos; to place points in an invisible environment, allowing them to discern the geometry.
		</p>
		
		<p class="text-lg">
			I used Godot's low-level PhysicsServer3D API for ray casting with little overhead, and the MultiMesh node to draw hundreds of thousands of dots with great performance.
		</p>
		
		<p class="text-lg">
			The dots are quads using a fragment shader to discard fragments beyond a radius and determine colour using world space position.
		</p>
		
		<video src="/lidar/demo.mp4" autoplay muted loop playsinline controls width="600" class="rounded-xl shadow-lg">
			<track kind="captions" />
		</video>
	</div>
</div>