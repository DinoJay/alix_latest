<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';

	$seo = {
		title: 'Sardine',
		description:
			'Artiste Popi Creations Meuble unique Design Furniture mini-series multidisciplinaire'
	};
	const imgs = [
		['/sardine.webp', 'sardine'],
		['/sardinecote.webp', 'sardine cote 1'],
		['/sardineface.webp', 'sardine face'],
		['/sardine-detail.webp', 'sardine detail']
	];

	const imgs2 = [
		['/sardine1.webp', 'Sardine 1'],
		['/sardine2.webp', 'Sardine 2'],
		['/sardines_5.webp', 'Sardine 5: Multiplex chêne']
	];
</script>

<div class=" p-3 md:p-12 items-center md:items-start">
	<div class="w-80 text-justify">
		<h1 class="text-3xl mb-1">Sardines aux tomates</h1>
		<h2 class="mb-2">Tabouret ou table d’appoint</h2>
		<div class=" text-sm text-gray-600">
			<p class="">Gravure des formes à la CNC, résine coulée en creux</p>
			<p class="">Multiplex - epoxy - pieds en acier laqué jaune</p>
			<p class="">Choix de la hauteur des pieds</p>
			<p>105€ - Disponibilités ci-dessous.</p>
		</div>
	</div>
	<div class="flex flex-col md:flex-row md:mt-12">
		<div class="order-1 grid md:mr-24 gap-4 grid-cols-2 grid-rows-2">
			{#each imgs as s, i}
				<LightBox srcs={imgs} start={i} style="width:10rem" className="h-40  object-cover" />
			{/each}
		</div>
		<img
			class="mini-series-table-mobile md:mini-series-table-desktop order-0 md:order-last mb-3 md:mb-0 max-w-series"
			src="/mesure.webp"
			alt="mesure"
		/>
	</div>

	<h2 class=" mt-12">Disponibilités du moment:</h2>
	<div class=" text-gray-600 flex mt-3">
		<div class=" ">
			{#each imgs2 as s, i}
				<LightBox srcs={imgs2} start={i} style="width:10rem" className="h-40  mb-3 object-cover" />
			{/each}
		</div>
		<div class="ml-3">
			<div class="h-40 flex items-center justify-center text-sm text-center mb-3">
				<s>Sardine 1: <br />Multiplex bouleau</s>
			</div>
			<div class="h-40 flex items-center justify-center text-sm text-center">
				<s>Sardine 2: <br /> Multiplex bouleau</s>
			</div>
			<div class="h-40 flex items-center justify-center text-sm text-center">
				<s>Sardine 5: <br /> Multiplex chêne</s>
			</div>
		</div>
	</div>
</div>

<style>
</style>
