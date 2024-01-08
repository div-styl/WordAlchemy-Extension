<script>
	import { Searchbar } from '$lib';

	let title_home = 'Wordalchemy Extension';
	let description = 'My Chrome Extension for English Dictionary';
</script>

<svelte:head>
	<title>{title_home}</title>
	<meta name="description" content={description} />
</svelte:head>

<section class="pt-20">
	<!--	<div bind:this={lottieElement} class="h-[100px]" />-->
	<h1 class="text-3xl font-bold text-center ">Wordalchemy</h1>
	<Searchbar />
</section>

