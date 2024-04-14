<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';
	import FurnitureView from '../../../lib/FurnitureView.svelte';

	$seo = {
		title: 'Marée basse',
		description:
			'Artiste Popi Creations Meuble unique Design Furniture mini-series multidisciplinaire'
	};
	const imgs = [
		['/tableahut.webp', 'tableahaut'],
		['/detail1.webp', 'table detail 1'],
		['/detail2.webp', 'table detail 2'],
		['/tablecentre.webp', 'table detail 2']
	];
</script>

<FurnitureView
	title="Marée basse"
	subTitle="Table basse"
	descr="Gravure des formes à la CNC, marqueterie de laiton"
	materials="Multiplex bouleau - hêtre - epoxy - laiton"
	price="450€/table - dispo: 2"
	availability="2 Disponibles"
	{imgs}
	drawingImg="/table_plan.webp"
/>
