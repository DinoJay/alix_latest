<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';
	import FurnitureView from '../../../lib/FurnitureView.svelte';

	$seo = {
		title: 'Pions',
		description:
			'Artiste Popi Creations Meuble unique Design Furniture mini-series multidisciplinaire'
	};
	const imgs = [
		['/roireine.webp', 'roi renne'],
		['/foujaune.webp', 'fou jaune 1'],
		['/foubleu.webp', 'fou bleu'],
		['/pionjaunebleu.webp', 'pions jaune'],
		['/situation1.webp', 'situation 1'],
		['/situation2.webp', 'situation 2']
	];
</script>

<FurnitureView
	title="Pions"
	subTitle="Ensemble de pions pour jeu d'echec"
	descr="Découpe des formes à la laser dans du plexi transparent"
	materials="hêtre - plexi recyclé"
	price="60€ - Disponibilités ci-dessous (ou sur commande). Possibilités d'envoi (Frais non inclus)"
	availability="1 disponible"
	{imgs}
	drawingImg="/gabarie.webp"
/>
