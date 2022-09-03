<script>
	import { onMount } from 'svelte';
	import { createScene } from '../lib/scene.js';

	let el;

	onMount(() => {
		createScene(el);
	});
</script>

<svelte:head>
	<title>Three.js Svelte Boilerplate</title>
	<meta name="description" content="Three.js example app built with Svelte" />
</svelte:head>

<canvas bind:this={el} />
