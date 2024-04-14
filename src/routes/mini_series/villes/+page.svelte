<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';
	import FurnitureView from '../../../lib/FurnitureView.svelte';

	$seo = {
		title: 'Ville',
		description: 'Artiste Popi Creations Meuble unique Design Furniture multidisciplinaire'
	};
	const imgs = [
		['/ville1.webp', 'ville'],
		['/ville2.webp', 'ville'],
		['/ville3.webp', 'ville'],
		['/ville4.webp', 'ville'],
		['/ville5.webp', 'ville'],
		['/ville6.webp', 'ville'],
		['/ville7.webp', 'ville']
	];
</script>

<FurnitureView
	title="Villes"
	subTitle="Table Basse"
	descr="Gravure des formes à la CNC, résine coulée à plat"
	materials="Multiplex - epoxy - pieds en acier laqué jaune ou rouge"
	price="570€ / Table"
	availability="sur commande"
	{imgs}
	drawingImg="/ville-taille.webp"
/>
