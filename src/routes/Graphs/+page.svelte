<script>
	import pie_chart from '$lib/assets/pie_chart.png';
	import bar_project_count from '$lib/assets/bar_project_count.png';
	import bar_region_count from '$lib/assets/bar_region_count_stacked2.png';
	import bar_region_funds from '$lib/assets/bar_region_funds_stacked2.png';
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
		<div style="display:flex; justify-content:center;">
			<img alt="Pie Chart per Sector" src={pie_chart} style="width:50vw; min-width: 500px; margin-top:2vh; margin-bottom:5vh;"/>
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
		<img alt="Bar Chart per Sector" src={bar_project_count} style="width:70vw; min-width:500px; margin-bottom:4vh;"/>
	</div>
	<p style="margin:5px">It can be seen that the type of sustainability project that has the highest count are <b>Physical Connectivity</b> projects, with a count of 135.</p>
	<p style="margin:5px">The second highest is <b>Water Resources</b> at a count of 29.</p>
	<p style="margin:5px">Meanwhile, <b>Education</b> and <b>Power and Energy</b> have the lowest counts, with each at 1.</p>

	<br style="margin: 3vh 0">

	<h3>3. Which regions does the government prioritize?</h3>
	<div>
		<p><b>Bar chart illustrating the project counts of per region</b></p>
		<img alt="Bar Chart of projects per region" src={bar_region_count} style="width:80vw; min-width:500px; margin-bottom:4vh;"/>
	</div>

	<div>
		<p><b>Bar chart illustrating funds allocated for projects per region</b></p>
		<img alt="Bar Chart of funds per region" src={bar_region_funds} style="width:80vw; min-width:500px; margin-bottom:2vh;"/>
	</div>

	<p style="margin:5px"><i>Note that a single project may be implemented in more than one region, so there is double counting for the values.</i></p>
	<p style="margin:5px"><i>Additionally each region's count and funds does not include projects that are desginated as 'Nationwide'.</i></p>
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
