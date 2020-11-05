<script>
	import Nav from '../components/Nav.svelte';
	export let segment;
</script>

<style>
	main {
		height: 100vh;
		width: 100vw - 5rem;
		margin-left: 5rem;
		padding: 0;
		 
	}
	@media only screen and (max-width: 600px) {
		main {
			margin: 0 0 5rem 0;
			width: 100vw;
		}
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>