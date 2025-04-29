<script>
	import pie_legend from '$lib/assets/pie_legend.png';
	import pie from '$lib/assets/pie.png';
	import bar_sector_count from '$lib/assets/bar_sector_count.png';
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
	<h2>Project Graphs</h2>

	<h3>1. How are project funds allocated towards sustainability?</h3>
	<p>Total amount of funds allocated: <b>PHP 9.5684 Trillion</b></p>

	<div>
		<p><b>Pie Chart for percentage of funds allocated to each sector</b></p>
		<div class="row">
			<div class="column">
				<img alt="Pie Chart per Sector" src={pie} style="height:25vw"/>
			</div>
			<div class="column">
				<img alt="Pie Chart Legend" src={pie_legend} style="width:15vw"/>
			</div>
		</div>
	</div>

	<div>
		<p><b>Table for amount of funds allocated to each sector</b></p>
		<table>
			<tr>
				  <th>Sector</th>
				  <th>Indicative Project Cost (in Php B)</th>
				  <th>%</th>
			</tr>
			<tr>
				<td>Physical Connectivity</td>
				<td>8343.71</td>
				<td>87.20</td>
			</tr>
			<tr>
				<td>Water Resources</td>
				<td>775.07</td>
				<td>8.10</td>
			</tr>
			<tr>
				<td>Agriculture</td>
				<td>213.68</td>
				<td>2.23</td>
			</tr>
			<tr>
				<td>Health</td>
				<td>95.73</td>
				<td>1.00</td>
			</tr>
			<tr>
				<td>Digital Connectivity</td>
				<td>78.11</td>
				<td>0.82</td>
			</tr>
			<tr>
				<td>Education</td>
				<td>30.56</td>
				<td>0.32</td>
			</tr>
			<tr>
				<td>Other Infrastructure</td>
				<td>21.34</td>
				<td>0.22</td>
			</tr>
			<tr>
				<td>Power and Energy</td>
				<td>10.19</td>
				<td>0.10</td>
			</tr>
			<tr>
				<td>TOTAL</td>
				<td>95684</td>
				<td>100</td>
			</tr>
		</table>
	</div>

	<br style="margin: 3vh 0">

	<h3>2. What kind of sustainability projects is the current government focused on?</h3>
	<div>
		<p><b>Bar chart illustrating the project counts of each sector</b></p>
		<img alt="Pie Chart per Sector" src={bar_sector_count} style="width:60vw"/>
	</div>
	<p>It can be seen that the type of sustainability project that has the highest count are <b>Physical Connectivity</b> projects, with a count of 135. Meanwhile, the <b>Education</b> and <b>Power and Energy</b> have the lowest counts, with each at 1.</p>
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

	.row {
  		display: flex;
	}

	.column {
		flex: 33.33%;
		padding: 5vh;
	}

	table {
	border-collapse: collapse;
	width: 50vw;
	}

	td, th {
	border: 1px solid #000000;
	text-align: left;
	padding: 8px;
	}
</style>
