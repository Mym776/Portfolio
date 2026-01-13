<script>
	import favicon from '$lib/assets/favicon.svg';
	import Name from './App.svelte';
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>


<Name />