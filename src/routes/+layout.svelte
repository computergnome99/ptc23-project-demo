<script>
	import Navigation from '../components/navigation.svelte';
	import Footer from '../components/footer.svelte';
</script>

<div class="fixed top-0 w-screen z-10">
	<Navigation />
</div>

<main>
	<slot />
</main>

<Footer />
