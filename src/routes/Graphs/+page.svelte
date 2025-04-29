<script>
	import PieChart from '$lib/PieChart.svelte';
	import fund_allocation from '$lib/data/fund_allocation.json';

</script>

<svelte:head>
	<title>Graphs</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>Exploratory Data Analysis</h1>
</section>
<hr>

<section>
	<PieChart data={fund_allocation}/>
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
</style>
