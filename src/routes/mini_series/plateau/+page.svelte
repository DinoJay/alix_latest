<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';
	import FurnitureView from '../../../lib/FurnitureView.svelte';

	$seo = {
		title: 'Plateau',
		description:
			'Artiste Popi Creations Meuble unique Design Furniture mini-series multidisciplinaire'
	};

	const imgs = [
		['/plateauface.webp', 'table detail 0'],
		['/plateaufacejaune.webp', 'table detail 1'],
		['/plateaucote.webp', 'table detail 2'],
		['/plateau2.webp', 'table detail 3'],
		['/plateaudouble.webp', 'table detail 4']
	];
</script>

<FurnitureView
	title="Tableau"
	subTitle="Plateau"
	descr="Gravure des formes à la CNC, marqueterie de laiton."
	materials="Multiplex bouleau - epoxy - laiton"
	price="50€ / plateau"
	{imgs}
	availability="SOLD OUT"
	drawingImg="/plateau_plan.webp"
/>
