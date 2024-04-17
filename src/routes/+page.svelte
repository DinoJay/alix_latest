<script>
	import { seo } from '$lib/store.js';

	$seo = {
		title: 'Atelier Popi - Accueil',
		description: 'Popi Creations Meuble unique Design Furniture Atelier'
	};
</script>

<div class="flex gap-4 md:p-0 p-3 overflow-auto">
	<a
		class=" flex flex-col bg-cover flex-1 lg:home-el-width"
		href="/creations"
		style:background-image={'url("creations.webp")'}
	>
		<div class="creations-text text-center m-auto text-white font-sans uppercase">
			CRÉATIONS <br />UNIQUES
		</div>
	</a>
	<a
		class=" flex flex-col bg-cover lg:home-el-width flex-1"
		href="/mini_series"
		style:background-image={'url("decorsardine.webp")'}
	>
		<div class="collab-text m-auto font-sans uppercase text-center text-white">
			<span class="sm:hidden">Prod. <br />Multiples</span>
			<span class="hidden sm:block">Productions Multiples</span>
		</div>
	</a>
	<a class=" flex flex-col coin bg-fill lg:home-el-width flex-1" href="/coin">
		<div class=" collab-text m-auto font-sans uppercase text-center text-white">
			<span class="sm:block">Le Coin</span>
		</div>
	</a>
</div>

<style>
	.coin {
		background-color: #f2bf05;
	}
	a {
		/* width: 500px; */
		height: 500px;
	}
	/* .collab {
		min-width: 50%;
	} */

	.collab-text {
		font-size: 4rem;
	}
	.creations-text {
		font-size: 4rem;
	}
</style>
