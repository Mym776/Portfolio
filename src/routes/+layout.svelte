<script>
	import favicon from '$lib/assets/favicon.svg';
	import Name from './App.svelte';
	import Tile from './tile.svelte'
	let { children } = $props();

	let st = $state(["biking","golfing","swimming"])
	let colors = $state(["blue","red","green","grey","brown"])
	function s (){
		let temp = st.shift()
        st.push(temp)
		temp = colors.shift()
		colors.push(temp)
		temp = colors.shift()
		colors.push(temp)
		

	}
	setInterval(s, 3000);
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>


<Name />
<div>
	{#each st as h}
	<Tile hobby={h} color={colors[0]}/>
	{/each}
		
</div>

<style>
	div{
		display: flex;
		flex-direction: row;
		justify-content: space-around;
	}
</style>