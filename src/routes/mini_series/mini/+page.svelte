<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';

	$seo = {
		title: 'Table',
		description:
			'Artiste Popi Creations Meuble unique Design Furniture mini-series multidisciplinaire'
	};
	const imgs = [
		['/mini1.webp', 'mini 1'],
		['/mini2.webp', 'mini 2'],
		['/mini3.webp', 'mini 3'],
		['/mini4.webp', 'mini 4'],
		['/mini5.webp', 'mini 5'],
		['/mini6.webp', 'mini 6'],
		['/mini7.webp', 'mini 7'],
		['/mini8.webp', 'mini 8'],
		['/mini9.webp', 'mini 9']
	];
</script>

<div class=" p-3 md:p-12 items-center md:items-start">
	<div class="md:flex md:px-24">
		<div class="w-80">
			<h1 class="text-3xl mb-1">MINI</h1>
			<h2 class="mb-2">Tabouret pour enfant</h2>
			<div class="text-justify text-sm text-gray-600">
				<p class="">Gravure des formes à la CNC, résine coulée à plat.</p>
				<p class="mb-8">
					Multiplex chêne- epoxy - pieds en hêtre massif- Huile-vernis éco-responsable
				</p>
				<p class="mb-8">
					68€/ Tabouret - Disponibilités ci-dessous (ou sur commande). Possibilités d'envoi (Frais
					non inclus)
				</p>
				<div class="text-green-600">
					<p>Poisson 1: 1 disponibles</p>
					<p>Poisson 2: 3 disponibles</p>
					<p>Tomates: 0 disponibles</p>
				</div>
			</div>
		</div>
		<img class="mini-series-table-mobile m-auto md:ml-24 mt-12" alt="" src="/minitaille.webp" />
	</div>
	<div class="flex flex-row md:mt-12 gap-4 flex-wrap">
		{#each imgs as s, i}
			<LightBox srcs={imgs} start={i} className="h-40  w-40 object-cover " />
		{/each}
	</div>
</div>

<style>
</style>
