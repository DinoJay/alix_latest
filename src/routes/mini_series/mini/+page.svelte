<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';
	import FurnitureView from '../../../lib/FurnitureView.svelte';

	$seo = {
		title: 'Mini',
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

<FurnitureView
	title="MINI"
	subTitle="Tabouret pour enfant"
	descr="Gravure des formes à la CNC, résine coulée à plat."
	materials="Multiplex chêne- epoxy - pieds en hêtre massif- Huile-vernis éco-responsable"
	price="68€/ Tabouret - Disponibilités ci-dessous (ou sur commande). Possibilités d'envoi (Frais non inclus)"
	availability="
					Poisson 1: 1 disponibles,
					Poisson 2: 3 disponibles,
					Tomates: 0 disponibles "
	drawingImg="/minitaille.webp"
/>
