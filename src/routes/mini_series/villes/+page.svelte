<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';

	$seo = {
		title: 'Ville',
		description: 'Artiste Popi Creations Meuble unique Design Furniture multidisciplinaire'
	};
	const imgs = [
		['/ville.webp', 'ville'],
		['/ville1.webp', 'ville'],
		['/ville2.webp', 'ville'],
		['/ville3.webp', 'ville'],
		['/ville4.webp', 'ville'],
		['/ville5.webp', 'ville'],
		['/ville6.webp', 'ville'],
		['/ville7.webp', 'ville']
	];
</script>

<div class=" p-3 md:p-12 items-center md:items-start">
	<div class="w-80 text-justify">
		<h1 class="text-3xl mb-1">Villes</h1>
		<h2 class="mb-2">Table Basse</h2>
		<div class=" text-sm text-gray-600">
			<p>Gravure des formes à la CNC, résine coulée à plat</p>
			<p class="">Multiplex - epoxy - pieds en acier laqué jaune ou rouge</p>
			<p>570€ - Disponible sur commande.</p>
		</div>
	</div>
	<div class="flex flex-col md:flex-row md:mt-12">
		<div class="flex-none order-1 grid md:mr-24 gap-4 grid-cols-2 grid-rows-2">
			{#each imgs as s, i}
				<LightBox srcs={imgs} start={i} style="width:10rem" className="h-40  object-cover" />
			{/each}
		</div>
		<img
			class="mini-series-ville-mobile md:mini-series-ville-desktop order-0 md:order-last mb-3 md:mb-0 max-w-series"
			src="/ville-taille.webp"
			alt="ville"
		/>
	</div>
</div>
