<script>
	import { seo } from '$lib/store.js';

	$seo = {
		title: 'Productions-multiples',
		description:
			'Artiste Popi Creations Meuble Unique Design Furniture mini-series multidisciplinaire'
	};
</script>

<div class="md:p-12">
	<div class="p-3 max-w-xl">
		<h1 class="text-3xl mb-3">Productions multiples</h1>

		<p class="text-justify">
			Ici sont proposés des meubles ou objets où une machine numérique (CNC , Laser ) intervient
			dans une partie du processus de fabrication. Mais tout le reste est fait à la main! Ils sont
			donc tous légèrement différents et peuvent présenter de très légères imperfections. Dans la
			section "le coin", vous trouverez ceux qui ont des défauts de fabrication mais qui sont à prix
			réduit!
		</p>
	</div>

	<div class="sm:grid sm:grid-cols-2">
		<a class="md:p-12" href="/mini_series/mini">
			<img src="minicouv.webp" alt="rouget" />
		</a>
		<a href="/mini_series/sardine" class="">
			<img class="" src="sardinecouv.webp" alt="table" />
		</a>
		<a href="/mini_series/pion" class="">
			<img src="pionbleu.jpeg" alt="pionbleu" />
		</a>
		<a class="" href="/mini_series/rouget">
			<img src="rougetcouv.webp" alt="rougetcouv" />
		</a>
		<a class="" href="/mini_series/table">
			<img src="table.webp" alt="rouget" />
		</a>
		<a class="flex" href="/mini_series/villes">
			<img class="m-auto" src="ville.webp" alt="villes" />
		</a>
		<a class="" href="/mini_series/plateau">
			<img src="plateau.png" alt="plateau" />
		</a>
	</div>
</div>

<style>
	img {
		@apply p-12;
	}
</style>
