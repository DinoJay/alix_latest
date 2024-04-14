<script>
	import { seo } from '$lib/store.js';
	import LightBox from '$lib/LightBox.svelte';

	export let title;
	export let subTitle;
	export let descr;
	export let materials;
	export let price = '';
	export let priceCls = '';
	export let availability = '';

	export let drawingImg;

	export let imgs = [
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

<div class=" p-3 md:p-12 items-center md:items-start flex flex-col">
	<div class="md:flex">
		<div class="w-80">
			<h1 class="text-3xl mb-1">{title}</h1>
			<h2 class="mb-2">{subTitle}</h2>
			<div class="text-justify text-sm text-gray-600">
				<p class="">{descr}</p>
				<p class="mb-8">
					{materials}
				</p>
				<p class="mb-8 font-bold {priceCls}">
					{price}
				</p>
				<div class="text-green-600">
					{availability}
				</div>
			</div>
		</div>
		<img
			class="mini-series-table-mobile m-auto w-96 object-contain"
			style:height="370px"
			alt=""
			src={drawingImg}
		/>
	</div>
	<div class="grid grid-cols-1 lg:grid-cols-7 md:mt-12 gap-4 justify-items-center">
		{#each imgs as s, i}
			<LightBox srcs={imgs} start={i} className="h-80  w-full lg:w-40 lg:h-40 object-cover " />
		{/each}
	</div>
</div>

<style>
</style>
