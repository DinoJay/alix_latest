<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';

	$seo = {
		title: 'Pions',
		description:
			'Artiste Popi Creations Meuble unique Design Furniture mini-series multidisciplinaire'
	};
	const imgs = [
		['/roireine.webp', 'roi renne'],
		['/foujaune.webp', 'fou jaune 1'],
		['/foubleu.webp', 'fou bleu'],
		['/pionjaunebleu.webp', 'pions jaune'],
		['/situation1.webp', 'situation 1'],
		['/situation2.webp', 'situation 2']
	];
</script>

<div class=" p-3 md:p-12 items-center md:items-start">
	<div class="w-80 text-justify">
		<h1 class="text-3xl mb-1">Pions</h1>
		<h2 class="mb-2">Ensemble de pions pour jeu d'echec</h2>
		<div class=" text-sm text-gray-600">
			<p class="">Découpe des formes à la laser dans du plexi transparent</p>
			<p class="">hêtre - plexi</p>
			<p>60€ - Disponibilités ci-dessous (ou sur commande).</p>
			<p>Possibilités d'envoi</p>
		</div>
	</div>
	<div class="flex flex-col md:flex-row md:mt-12">
		<div class="order-1 grid md:mr-24 gap-4 grid-cols-2 grid-rows-2">
			{#each imgs as s, i}
				<LightBox srcs={imgs} start={i} style="width:10rem" className="h-40  object-contain" />
			{/each}
		</div>
		<img
			class="mini-series-table-mobile md:mini-series-table-desktop order-0 md:order-last mb-3 md:mb-0 max-w-series"
			src="/gabarie.webp"
			alt="gabarie"
		/>
	</div>
</div>

<style>
</style>
