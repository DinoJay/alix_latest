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

	$: imgs = [
		{ src: 'Tableverte.webp', href: '/table-verte', bg: '#f82f4e', title: 'Table Verte' },
		{
			src: 'meublecd.png',
			href: '/meublecd',
			bg: '#332fd8',
			cls: !grid ? 'p-24' : 'p-6',
			title: 'Vallorcines'
		},
		{ src: 'tic.webp', href: '/tic', bg: 'rgb(224, 118, 118)', title: 'Tic' },
		{ src: 'tablesunset.webp', href: '/sunset', bg: '#f9d413', title: 'Sunset' },
		{ src: 'table-2.webp', href: '/table-2', bg: 'dodgerblue', title: 'Grande Soeur' },
		{ src: 'table-1.webp', href: '/table-1', bg: 'tomato', title: 'Baby' },
		{ src: 'commode.webp', href: '/commode', bg: 'lightskyblue', title: 'Everest' },
		{ src: 'table-bleu.webp', href: '/table-bleu', bg: 'yellow', title: 'Tableu' },
		{ src: 'banc.webp', href: '/banc', bg: '#5cac92', title: 'Chaussette' },
		{ src: 'meuble entree.webp', href: '/meuble-entree', bg: '#f9b256', title: 'Entrée' },
		{ src: 'buffet.webp', href: '/buffet', bg: '#f82f4e', title: 'Clapier' }
	];
</script>

<div class=" absolute hidden right-0 top-0 flex z-10" style:height="40px">
	<button class="" on:click={gridClick}
		><img
			class=" mr-2 sm:mr-1 sm:mt-1"
			alt="grid"
			width="40"
			height="40"
			src="/gridicon.png"
		/></button
	>
</div>
<div
	class="flex-grow relative m-auto"
	class:grid={!grid}
	class:grid-cont={grid}
	class:grid-cols-1={!grid}
	class:sm:grid-cols-2={!grid}
	class:flex={grid}
	class:justify-center={grid}
	class:flex-wrap={grid}
	style:max-width={grid ? '700px' : null}
>
	{#each imgs as d (d.href)}
		<div animate:flip={{ duration: 200 }} class="img-cont mb-3 relative" style="background:{d.bg}">
			<a class="w-full overflow-hidden" href={d.href}>
				<img class={d.cls ? d.cls : ''} class:md:max-w-prose={!grid} src={d.src} alt={d.href} />
			</a>
			<div class="absolute bottom-0 left-0">
				<div class="ml-2 mb-3 text-xl uppercase bg-black text-white px-2">{d.title}</div>
			</div>
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
