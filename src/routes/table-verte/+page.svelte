<script>
	import ArrowLeftIcon from 'svelte-remixicon/lib/icons/ArrowLeftFill.svelte';
	import HomeIcon from 'svelte-remixicon/lib/icons/Home2Fill.svelte';
	import { seo } from '$lib/store.js';

	$seo = {
		title: 'Buffet',
		description: 'modulable Buffet Popi Creations Meuble unique Design Furniture Multiplex'
	};
</script>

<div class="flex flex-col">
	<div class="m-auto max-w-prose flex flex-col items-center p-3">
		<h1 class=" text-3xl uppercase text-center mb-3">TABLE VERTE</h1>
		<h2 class=" text-lg uppercase text-center mb-3">TABLE BASSE</h2>
		<div>Hêtre - Alupanel vert - Multiplex bouleau - Verre armé 40,2 x 89 x 44,7</div>
		<div>160 x 120 x 37,5</div>
		<img class="mb-20 mt-20" src="Tableverte-1.webp" alt="table verte 1" />
		<img class="mb-20" src="tableverte-2.webp" alt="table verte 2" />
		<img class="mb-20" src="Tableverte-3.webp" alt="table verte 3" />
		<img class="mb-20" src="Tableverte-4.webp" alt="table verte 4" />
		<img class="mb-20" src="Tableverte-5.webp" alt="table verte 5" />
		<div class="flex w-full items-center">
			<a class="mr-auto" href="/creations">
				<img height="40" width="40" src="home.webp" alt="home" />
			</a>
			<a class="/table-2" href="/meublecd">
				<img height="40" width="40" src="arrow-right.webp" alt="arrow left" />
			</a>
		</div>
	</div>
</div>

<style>
	img {
		@apply px-1;
	}
	h1 {
		color: #1d6e31;
	}
</style>
