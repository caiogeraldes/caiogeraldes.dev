<script lang="ts">
	import Navbar from '$lib/Navbar.svelte';
	import Footer from '../lib/Footer.svelte';
	import Header from '../lib/Header.svelte';
	import Menu from '../lib/Menu.svelte';

	let fName = 'Caio';
	let lName = 'Geraldes';
	let description = 'Doutorando em Letras Clássicas';
	// let lang = "pt-br";
</script>

<main>
	<Navbar />
	<Header {fName} {lName} {description} />
	<Menu />
	<slot />
	<Footer />
</main>

<style>
	main {
		min-height: 100vh;
		display: flex;
		flex-direction: column;
		padding-bottom: 5rem;
	}
</style>
