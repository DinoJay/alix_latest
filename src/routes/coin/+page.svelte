<script>
	// import '../styles/tailwind.css';

	import { seo } from '$lib/store.js';
	import { flip } from 'svelte/animate';

	$seo = {
		title: 'Le Coin',
		description: 'Popi Creations Meuble unique Design Furniture'
	};
</script>

<h1 class="text-lg">Under Construction...</h1>
<div class="max-w-prose">
	Ici vont ^etre disposés ceux qui ont un ou des défauts mais qui ne sont pas pour autant ratés ! Et
	oui, on a beau roder du mieux qu'on peut la technique m^eme après plusieurs tests, il arrive
	toujours des surprises... Mais les prix sont donc plus doux ici .
</div>

<style>
	/* #first {
		@apply flex;
		@apply justify-center;
		/* @apply w-full; */
	/* background-size: 100% auto; */
	/* background-repeat: no-repeat; */
	/* background-color: dodgerblue; */
	/* } */
	.img-cont {
		@apply bg-center;
		@apply flex;
		@apply justify-center;
		/* @apply w-full; */
		/* background-size: 100% auto; */
		background-repeat: no-repeat;
		/* background-color: tomato; */
	}

	.grid-cont div {
		width: 200px;
		height: 200px;
	}

	@media screen and (max-width: 600px) {
		.grid-cont div {
			width: 150px;
			height: 150px;
		}
	}
</style>
