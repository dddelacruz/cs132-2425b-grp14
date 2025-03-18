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
	<h2>Main Research Question:</h2>
	<p>How does the Philippine government allocate funds for sustainability projects, and what priorities are their current priorities? </p>

	<h2>Background of the Study</h2>
	<p>SGD 11 goal is to “Make Cities and Human Settlements Inclusive, Safe, Resilient, and Sustainable”. According to the United Nations, this SDG tackles problems related to transport, housing, and sustainable development such as Disaster Risk Reduction, accessibility, and minimization of environmental impact. Key performance indicators are used to quantify the SDG and according to the SDG watch released by the Philippine Statistics Authority, the Philippines is far from reaching the desired goals for 2023. These indicators include 11.1.1p1 or Proportion of urban population who are informal settlers, 11.5.1 or Number of deaths, missing persons and directly affected persons attributed to disasters per 100,000 population 5, and 11.6.2.p1 or Percentage of highly urbanized and other major urban centers within ambient air quality guidelines value increased among others . This study uses a dataset from NEDA which contains the state current and future projects of the Philippines to investigate the different projects being implemented by the government.
	</p>

	<h2>Description of Research Problems</h2>
	<h3>How are project funds allocated towards sustainability?</h3>
	<ul>
		<li>Investigate how funds are distributed between sustainability projects as opposed to other projects</li>
	</ul>
	
	<h3>What kind of sustainability projects is the current government focused on?</h3>
	<ul>
		<li>Investigate how funds are distributed between different sustainability projects</li>
	</ul>

	<h3>Which sectors/regions does the government prioritize?</h3>
	<ul>
		<li>Investigate the distribution of funds according to location.</li>
	</ul>

	<h2>Hypotheses</h2>
	<p><b>Null Hypothesis:</b> The government is not prioritizing certain kinds of sustainability projects.</p>
	<p><b>Alternate Hypothesis:</b> The government is prioritizing certain kinds of sustainability projects. </p>

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
