<script>
	import Icon from '$lib/assets/Icon.svg';
	import Theme from './theme/selecte.svelte';
</script>

<nav class="border-b-[1px] border-blue-600/25 dark:border-b-0">
	<div class="max-w-screen-xl justify-between flex mx-auto p-3 space-x-10">
		<a href="/" class="flex items-start justify-start">
			<img src={Icon} class="h-7 w-7" alt="WordAlchemy Logo" />
			<span class="text-xl font-semibold mx-2">wordalchemy</span>
		</a>
		<div class="pt-1">
			<Theme />
		</div>
		
	</div>
</nav>
