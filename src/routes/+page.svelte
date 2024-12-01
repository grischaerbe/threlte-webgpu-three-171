<script lang="ts">
	import { Canvas } from '@threlte/core';
	import { WebGPURenderer } from 'three/webgpu';
	import Scene from './Scene.svelte';
</script>

<main>
	<Canvas
		createRenderer={(canvas) => {
			return new WebGPURenderer({ canvas });
		}}
	>
		<Scene />
	</Canvas>
</main>

<style>
	:global(html, body) {
		margin: 0;
		padding: 0;
	}

	main {
		width: 100vw;
		height: 100vh;
	}
</style>
