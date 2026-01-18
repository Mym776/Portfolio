<script>
	import favicon from '$lib/assets/favicon.svg';
	import Name from './App.svelte';
	import Tile from './tile.svelte'
	let { children } = $props();

	let st = $state(["biking","golfing","swimming"])

	function s (){
		let temp = st.shift()
        st.push(temp)
		
	}
	setInterval(s, 3000);

</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>


<Name />
<div>
	<Tile hobby={st[0]}/>
	<Tile hobby={st[1]}/>
	<Tile hobby={st[2]}/>	
</div>

<style>
	div{
		display: flex;
		flex-direction: row;
		justify-content: space-around;
	}
</style>