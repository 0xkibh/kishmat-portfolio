<script>
	import "../app.css";
	import Header from './Header.svelte';
</script>

<div class="app h-screen">
	<Header />

	<main class="">
		<slot />
	</main>
</div>

<style>
	
</style>
