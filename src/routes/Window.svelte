<script lang="ts">
	export let left = 100;
	export let top = 100;

	let moving = false;

	function onMouseDown() {
		moving = true;
		// Bring this window to the front
		const windows = document.querySelectorAll(".window");
		windows.forEach((window) => {
			window.classList.remove("active");
		});
		const currentWindow = document.querySelector(".window");
		if (currentWindow) {
			currentWindow.classList.add("active");
		}
	}

	function onMouseMove(e: MouseEvent) {
		if (moving) {
			left += e.movementX;
			top += e.movementY;
		}
	}

	function onMouseUp() {
		moving = false;
	}
</script>

<section class="window glass active" style="width: 300px; left: {left}px; top: {top}px;">
	<div role="presentation" class="title-bar" on:mousedown={onMouseDown}>
		<div class="title-bar-text">A Window</div>
		<div class="title-bar-controls">
			<button aria-label="Minimize"></button>
			<button aria-label="Maximize"></button>
			<button aria-label="Close"></button>
		</div>
	</div>
	<div class="window-body has-space">
		<p>This is some text inside a window</p>
	</div>
</section>

<svelte:window on:mouseup={onMouseUp} on:mousemove={onMouseMove} />

<style>
	.window {
		user-select: none;
		position: absolute;
	}

	.violet::before,
	.violet > .title-bar {
		background-color: #805ba5;
	}
</style>
