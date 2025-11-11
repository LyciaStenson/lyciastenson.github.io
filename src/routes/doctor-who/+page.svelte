<title>Doctor Who | Lycia Stenson</title>

<div class="space-y-5">
	<h1 class="text-5xl font-bold">
		Doctor Who
	</h1>
	
	<p class="text-lg">
		Doctor Who demos featuring a &apos;Weeping Angel&apos; that only moves when not in the player's view, and a TARDIS which appears bigger-on-the-inside through a portal system.
	</p>
	
	<div class="space-y-2">
		<video src="/doctor-who/angel.mp4" autoplay muted loop playsinline controls width="600" class="rounded-xl shadow-lg">
			<track kind="captions" />
		</video>
		
		<p class="text-lg">
			The &apos;Weeping Angel&apos; uses Godot's VisibleOnScreenNotifier3D node to detect whether the angel is in the camera's view frustrum. In the case that it is, it also uses ray casts to check if the angel is obscured.
		</p>
		<p class="text-lg">
			If the angel is obscured or outside the view frustrum, the angel pathfinds to the player.
		</p>
	</div>
	
	<div class="space-y-2">
		<video src="/doctor-who/tardis.mp4" autoplay muted loop playsinline controls width="600" class="rounded-xl shadow-lg">
			<track kind="captions" />
		</video>
		
		<p class="text-lg">
			The TARDIS uses a custom portal system to make the police box appear bigger on the inside. A camera is placed relative to the destination portal with the same position and rotation as the player's camera relative to the origin portal.
		</p>
	</div>
	
	<div class="space-y-2">
		<img src="/doctor-who/portal-issue.jpg" width="600" alt="Portal issue" />
		
		<p class="text-lg">
			Godot does not support oblique near clipping planes, which are required for portals to render only what is in front of them. This means the back of the police box obstructs the view of the portal seen from inside the TARDIS.
		</p>
		<p class="text-lg">
			I plan to implement a proper portal system in my custom engine, <a class="font-semibold" href="/nightbird">Nightbird</a>, in the future.
		</p>
	</div>
	
	<div class="space-y-0">
		<p class="text-lg">
			Asset Credits
		</p>
		<ul class="list-disc pl-8 space-y-1">
			<li><a class="font-bold" href="https://skfb.ly/6Toxr">12th Doctor's Tardis Exterior</a> by Ewan Lejkowski, licensed under CC BY 4.0</li>
		</ul>
	</div>
</div>