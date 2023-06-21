<script>
	import img1 from "../images/bg.webp";
	import img2 from "../images/collageImage1.webp";
	import img3 from "../images/collageImage2.webp";
	import img4 from "../images/collageImage3.webp";
	let images = [img1, img2, img3, img4];

	let heading = images[0];

	setInterval(() => {
		heading = images[Math.floor(Math.random() * 4)];
	}, 2000);
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>

		<img class="image" src={heading} alt="" srcset="" />
	</h1>
</section>

<style>
	.image {
		width: 90%;
		height: 500px;
		aspect-ratio: 16/9;
		margin: auto;
		display: block;
		border-radius: 30px;
		-webkit-box-shadow: 10px 10px 75px 0px rgba(0, 0, 0, 0.75);
		-moz-box-shadow: 10px 10px 75px 0px rgba(0, 0, 0, 0.75);
		box-shadow: 10px 10px 75px 0px rgba(0, 0, 0, 0.75);
	}
</style>
