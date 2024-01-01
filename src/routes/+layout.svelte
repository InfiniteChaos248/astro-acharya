<script>
	import Header from "./Header.svelte";
</script>

<div class="app">
	<Header/>

	<main>
		<slot />
	</main>
</div>

<style>	
    .app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;		
		margin: -8px;
		background-color: #FCF5E5;
	}

	main {
		padding-left: 5px;
		padding-right: 5px;
		padding-top: 5px;
	}
</style>