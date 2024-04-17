<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';
	import FurnitureView from '../../../lib/FurnitureView.svelte';

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

<FurnitureView
	title="Rougets aux citrons"
	subTitle="Tabouret ou table d’appoint"
	descr="Gravure des formes à la CNC, résine coulée en creux"
	materials="Multiplex - epoxy - pieds en acier laqué bleu"
	price="140€ / Table - Disponibilités ci-dessous (ou sur commande). Possibilités d'envoi (Frais non inclus)"
	availability="Sur Commande"
	{imgs}
	drawingImg="/mesure.webp"
/>
