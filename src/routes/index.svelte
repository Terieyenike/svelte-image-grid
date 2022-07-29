<script>
	let images = [
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1659047063/image-grid/wasa-crispbread-f4kKHjf1Ke8-unsplash.jpg',
			id: 1
		},
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1659047062/image-grid/wasa-crispbread-0P-cY9tUNnY-unsplash.jpg',
			id: 2
		},
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1659047062/image-grid/toa-heftiba-ZPIDk9h-kig-unsplash.jpg',
			id: 3
		},
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1659047061/image-grid/niels-erdmann-klO77jxxlYw-unsplash.jpg',
			id: 4
		},
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1659047061/image-grid/komarov-egor-Lc2R_w0zvtA-unsplash.jpg',
			id: 5
		},
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1659047061/image-grid/loume-visser-lDCm3Aw3m0I-unsplash.jpg',
			id: 6
		},
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1659047061/image-grid/hans-isaacson-7Hfe18-OIB0-unsplash.jpg',
			id: 7
		},
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1659047061/image-grid/giancarlo-corti-hWpHAslIJjc-unsplash.jpg',
			id: 8
		},
		{
			img: 'https://res.cloudinary.com/terieyenike/image/upload/v1651446129/image-grid/pexels-tobi-758773_sydxon.jpg',
			id: 9
		}
	];
</script>

<main>
	<h1 class="flex justify-center capitalize text-3xl mt-4 font-bold underline">image grid</h1>
	<div
		class="container mx-auto grid lg:grid-cols-3 md:grid-cols-2 xl:grid-cols-2 gap-8 py-10 w-11/12 max-w-7xl"
	>
		{#each images as image (image.id)}
			<div class="w-full rounded">
				<img src={image.img} alt="grid placeholder images" class="shadow-md" />
			</div>
		{/each}
	</div>
	<footer class="flex justify-center capitalize mb-4 text-gray-500">
		made with tailwind CSS and svelte
	</footer>
</main>
