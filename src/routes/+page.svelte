<script lang="ts">
	import { onMount } from 'svelte';
	import { createScene } from '$lib/scene';

	let el:HTMLCanvasElement;

	onMount(() => {
		createScene(el);
	});
</script>

<svelte:head>
	<title>Three.js Sveltekit</title>
	<meta name="description" content="Three.js example app built with Svelte" />
</svelte:head>

<canvas bind:this={el} />
