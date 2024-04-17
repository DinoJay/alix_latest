<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';
	import FurnitureView from '../../../lib/FurnitureView.svelte';

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

<FurnitureView
	title="Sardines aux tomates"
	subTitle="Table d'appoint - Tabouret"
	descr="Gravure des formes à la CNC, résine coulée en creux"
	materials="Multiplex chêne - epoxy - pieds en acier laqué jaune - Huile/vernis éco-responsable"
	price="140€/ Table, Tabouret - Disponibilités ci-dessous (ou sur commande). Possibilités d'envoi (Frais non inclus)"
	availability="1 disponible"
	imgHeight="280px"
	{imgs}
	drawingImg="/sardine-mesure.webp"
/>
