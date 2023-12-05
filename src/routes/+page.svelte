<script>
	import {Searchbar} from '$lib';
	let extensiontitle = 'Wordalchemy Extension';
	let description = 'My Chrome Extension for English Dictionary';
</script>

<svelte:head>
	<title>{extensiontitle}</title>
	<meta name="description" content={description} />
</svelte:head>

<section >
	<Searchbar />
</section>

