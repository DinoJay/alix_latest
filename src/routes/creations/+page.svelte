<script>
	// import '../styles/tailwind.css';

	import { seo } from '$lib/store.js';

	$seo = {
		title: 'Creations',
		description: 'Popi Creations Meuble unique Design Furniture'
	};
	let grid = false;
	let gridClick = () => (grid = !grid);

	const imgs = [
		{ src: 'tic.webp', href: '/tic', bg: 'rgb(224, 118, 118)' },
		{ src: 'tablesunset.webp', href: '/sunset', bg: '#f9d413' },
		{ src: 'table-2.webp', href: '/table-2', bg: 'dodgerblue' },
		{ src: 'table-1.webp', href: '/table-1', bg: 'tomato' },
		{ src: 'commode.webp', href: '/commode', bg: 'lightskyblue' },
		{ src: 'table-bleu.webp', href: '/table-bleu', bg: 'yellow' },
		{ src: 'banc.webp', href: '/banc', bg: '#5cac92' },
		{ src: 'meuble entree.webp', href: '/meuble-entree', bg: '#f9b256' },
		{ src: 'buffet.webp', href: '/buffet', bg: '#f82f4e' }
	];
</script>

<div class="flex-grow relative {grid && 'flex flex-wrap grid-cont'}">
	<div class=" absolute hidden right-0 top-0 flex">
		<button class="m-auto" on:click={gridClick}
			><img class="" alt="grid" width="40" height="40" src="/gridicon.png" /></button
		>
	</div>
	{#each imgs as d}
		<div class="img-cont mb-3" style="background:{d.bg}">
			<a href={d.href}>
				<img class="md:max-w-prose" src={d.src} alt={d.href} />
			</a>
		</div>
	{/each}
</div>

<style>
	/* #first {
		@apply flex;
		@apply justify-center;
		/* @apply w-full; */
	/* background-size: 100% auto; */
	/* background-repeat: no-repeat; */
	/* background-color: dodgerblue; */
	/* } */
	.img-cont {
		@apply bg-center;
		@apply flex;
		@apply justify-center;
		/* @apply w-full; */
		/* background-size: 100% auto; */
		background-repeat: no-repeat;
		/* background-color: tomato; */
	}

	.grid-cont div {
		max-width: 200px;
		height: 200px;
	}
</style>
