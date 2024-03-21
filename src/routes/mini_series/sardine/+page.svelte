<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';

	$seo = {
		title: 'sardine',
		description:
			'Artiste Popi Creations Meuble unique Design Furniture mini-series multidisciplinaire'
	};
	const imgs = [
		['/sardine1.webp', 'sardine 1'],
		['/sardine2.webp', 'sardine 2'],
		['/sardine3.webp', 'sardine 3'],
		['/sardine4.webp', 'sardine 4']
	];
</script>

<div class=" p-3 md:p-12 items-center md:items-start">
	<div class="md:flex md:px-24">
		<div class="w-80">
			<h1 class="text-3xl mb-1 uppercase">Sardines aux tomates</h1>
			<h2 class="mb-2">Table d'appoint - Tabouret</h2>
			<div class="text-justify text-sm text-gray-600">
				<p class="">Gravure des formes à la CNC, résine coulée à plat.</p>
				<p class="mb-8">
					Multiplex chêne - epoxy - pieds en acier laqué jaune - Huile/vernis éco-responsable
				</p>
				<p class="mb-8">
					105€/ Table, Tabouret - Disponibilités ci-dessous (ou sur commande). Possibilités d'envoi
					(Frais non inclus)
				</p>
				<div class="text-green-600">
					<p>2 disponibles</p>
				</div>
			</div>
		</div>
		<img
			style:height="270px"
			class="mini-series-table-mobile md:ml-24 w-96 mt-12 object-contain"
			alt=""
			src="/sardinetaille.webp"
		/>
	</div>
	<div class="flex flex-col md:flex-row md:mt-12 gap-4 flex-wrap justify-center">
		{#each imgs as s, i}
			<LightBox srcs={imgs} start={i} className="h-40  w-40 object-cover " />
		{/each}
	</div>
</div>

<style>
</style>
