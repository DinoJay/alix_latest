<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';

	$seo = {
		title: 'Rouget',
		description:
			'Artiste Popi Creations Meuble unique Design Furniture mini-series multidisciplinaire'
	};
	const imgs = [
		['/rouget.webp', 'sardine'],
		['/rougetcote.webp', 'sardine cote 1'],
		['/rougetface.webp', 'sardine face'],
		['/sardine-detail.webp', 'rouget detail']
	];
	const imgs2 = [
		['/rouget3.webp', 'rouget 3'],
		['/rouget4.webp', 'rouget 4'],
		['/detail.webp', 'detail'],
		['/rouget_6.webp', 'rouget 6'],
		['/rouget_7.webp', 'rouget 7']
	];
</script>

<div class=" p-3 md:p-12 items-center md:items-start">
	<div class="w-80 text-justify">
		<h1 class="text-3xl mb-1">Rougets aux citrons</h1>
		<h2 class="mb-2">Tabouret ou table d’appoint</h2>
		<div class="text-sm text-gray-600">
			<p class="">Gravure des formes à la CNC, résine coulée en creux</p>
			<p class="">Multiplex - epoxy - pieds en acier laqué bleu</p>
			<p class="">Choix de la hauteur des pieds</p>
			<p>105€ - Disponibilités ci-dessous (ou sur commande).</p>
			<p>Possibilités d'envoi</p>
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
			alt="mesure"
			src="/mesure.webp"
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
				<s>Rouget 3: <br />Multiplex bouleau</s>
			</div>
			<div class="h-40 flex items-center justify-center text-sm text-center mb-3">
				Rouget 4: <br /> Multiplex pin pologne <br /> 85€ <br /> défaut: voir <br /> photo ci-après
			</div>
			<div class="h-40 flex items-center justify-center text-sm text-center mb-3">
				Le rouge est <br /> légèrement infiltré <br /> dans la fibre du bois
			</div>
			<div class="h-40 flex items-center justify-center text-sm text-center mb-3">
				<div><s>Rouget 6: <br />Multiplex chêne</s></div>
			</div>
			<div class="h-40 flex items-center justify-center text-sm text-center">
				<div>Rouget 7:<br />Multiplex pin de Pologne</div>
			</div>
		</div>
	</div>
</div>

<style>
</style>
