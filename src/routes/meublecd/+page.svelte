<script>
	import { seo } from '$lib/store.js';

	$seo = {
		title: 'Table Sunset',
		description: 'Popi Creations Meuble unique Design Furniture Table Moderne Hetre Plexi Couleur'
	};
</script>

<div class="flex flex-col">
	<div class="sm:min-w-prose m-auto max-w-prose flex flex-col items-center p-3">
		<h1 class="mx-auto text-3xl uppercase text-center mb-3">Mont Blanc</h1>
		<h2 class="mx-auto text-lg uppercase text-center mb-3">Étagère à CD</h2>

		<div class="text-center flex flex-col justify-center">
			<p>Hêtre - Plexi fluo - Multiplex chêne</p>
			<p>87 x 84 x 18</p>
			<p class="mt-6 text-gray-600">
				Meuble réalisé pour une commande pour ranger une collection de CDs. Les plexis ont été
				récupérés sur la table "Sunset" qui elle est transformée en une nouvelle table. Ce meuble
				est parti pas loin du Mont Blanc. Les dessins sur les portes en plexi représentent ce
				dernier sous différents points de vue.
			</p>
		</div>
		<img class="mt-32" src="CD1.webp" alt="cd" />
		<img class="my-32" src="CD2.webp" alt="cd2" />
		<img class="" src="CD3.webp" alt="cd3" />
		<img class="mt-32" style="" src="CD4.webp" alt="cd4" />
		<img class="mt-32" src="CD5.webp" alt="cd5" />
		<img class="mt-32 mb-12" src="CD6.webp" alt="cd6" />
		<div class="flex w-full justify-center items-center mb-3">
			<a class="/creations" href="/creations">
				<img height="40" width="40" src="home.webp" alt="home" />
			</a>
			<a class="ml-auto" href="/tic">
				<img height="40" width="40" src="arrow-right.webp" alt="arrow right" />
			</a>
		</div>
	</div>
</div>

<style>
	h1 {
		color: #332fd8;
	}

	img {
		@apply px-1;
	}

	.situation {
		/* @apply px-12; */
	}
</style>
