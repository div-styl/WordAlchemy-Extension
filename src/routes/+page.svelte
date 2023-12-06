<script>
	import {Searchbar} from '$lib';
	import { Cat } from '$lib';
	import { onMount } from 'svelte';
	let extensiontitle = 'Wordalchemy Extension';
	let description = 'My Chrome Extension for English Dictionary';

	let lottieElement;

	onMount(() => {
		import('lottie-web').then((lottie) => {
			// Load and display the Lottie animation
			const animation = lottie.loadAnimation({
				container: lottieElement,
				loop: true, // Set to true if you want the animation to loop
				autoplay: true, // Set to true if you want the animation to play automatically
				animationData: Cat // Replace with your Lottie animation data
			});

			return () => {
				// Cleanup when the component is unmounted
				animation.destroy();
			};
		});
	});

</script>

<svelte:head>
	<title>{extensiontitle}</title>
	<meta name="description" content={description} />
</svelte:head>

<section>
	<div bind:this={lottieElement} class="h-[100px]" />
	<Searchbar />
</section>

