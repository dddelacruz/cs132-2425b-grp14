<script>
	import Counter from '$lib/Counter.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>CS 132 2425B Portfolio</h1>
	<h2>Group 14 - Sustainability</h2>
	<h2>DE LA CRUZ, MACARAIG, FADRI</h2>
</section>

<section>
	<h1>Research Design</h1>
	<h2>Research Questions</h2>
</section>

<section>
	<h1>About the Dataset</h1>
</section>

<section>
	<a href="https://docs.google.com/spreadsheets/d/1REc2vacPZloKL9R9SHjVuz4Ega1yfvli4pcqteynxzs" style="font-size:2.5em">
		Link to the Dataset
	</a>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
