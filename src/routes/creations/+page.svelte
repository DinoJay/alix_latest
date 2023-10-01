<script>
	// import '../styles/tailwind.css';

	import { seo } from '$lib/store.js';
	import { flip } from 'svelte/animate';

	$seo = {
		title: 'Creations',
		description: 'Popi Creations Meuble unique Design Furniture'
	};
	let grid = false;
	let gridClick = (e) => {
		e.stopPropagation();

		grid = !grid;
	};

	const imgs = [
		{ src: 'meublecd.png', href: '/meublecd', bg: '#332fd8' },
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

<div class=" absolute right-0 top-0 flex z-10" style:height="40px">
	<button class="" on:click={gridClick}
		><img class="mt-2 mr-3 sm:mr-0" alt="grid" width="40" height="40" src="/gridicon.png" /></button
	>
</div>
<div
	class="flex-grow relative m-auto"
	class:grid-cont={grid}
	class:flex-grid={!grid}
	class:flex={grid}
	class:justify-center={grid}
	class:flex-wrap={grid}
	style:max-width={grid ? '700px' : null}
>
	{#each imgs as d (d.href)}
		<div
			animate:flip={{ duration: 200 }}
			class="img-cont mb-3"
			class:mr-3={grid}
			style="background:{d.bg}"
		>
			<a href={d.href}>
				<img class:md:max-w-prose={!grid} src={d.src} alt={d.href} />
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
		width: 200px;
		height: 200px;
	}

	@media screen and (max-width: 600px) {
		.grid-cont div {
			width: 150px;
			height: 150px;
		}
	}
</style>
