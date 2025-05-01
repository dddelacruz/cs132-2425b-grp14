<script>
	import pie_chart from '$lib/assets/pie_chart.png';
	import bar_project_count from '$lib/assets/bar_project_count.png';
	import bar_region_count from '$lib/assets/bar_region_count_stacked2.png';
	import bar_region_funds from '$lib/assets/bar_region_funds_stacked2.png';
	import pnr from '$lib/assets/pnr.png';
	import train from '$lib/assets/train.png';
	import airplane from '$lib/assets/airplane.png';
	import road from '$lib/assets/road.png';
	import hotspots from '$lib/assets/hotspots.png';
</script>

<svelte:head>
	<title>EDA</title>
	<meta name="description" content="Exploratory Data Analysis Page" />
</svelte:head>

<section>
	<h1>Exploratory Data Analysis</h1>
</section>

<hr>

<section>
	<h2>Project Graphs</h2>

	<h3>1. How are project funds allocated towards sustainability?</h3>
	<p>Total amount of funds allocated: <span class='highlight'>PHP 9.5684 Trillion</span></p>

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

	<br>

	<p>It can be seen that the sector that is most invested on is <span class='highlight'>Physical Connectivity</span>, with the majority of funds allocated going towards it.</p>
	<p>Investigating further to see the ten most expensive projects:</p>

	<br>

	<div>
		<p><b>Table containing the ten most expensive projects</b></p>
		<table style='width:70vw'>
			<tr>
				  <th>Rank</th>
				  <th>Project Title</th>
				  <th>Sector</th>
				  <th>Indicative Project Cost (in Php B)</th>
				  <th>Region/s</th>
			</tr>
			<tr>
				<td>1</td>
				<td>North-South Commuter Railway (PNR North 1,PNR North 2,PNR South Commuter)</td>
				<td>Physical Connectivity</td>
				<td>873.62</td>
				<td>NCR, III, IV-A</td>
			</tr>
			<tr>
				<td>2</td>
				<td>New Manila International Airport (Bulacan International Airport)</td>
				<td>Physical Connectivity</td>
				<td>735.63</td>
				<td>III</td>
			</tr>
			<tr>
				<td>3</td>
				<td>Subic-Clark-Manila-Batangas Dedicated Rail Corridor Formerly 'Subic Clark Railway'</td>
				<td>Physical Connectivity</td>
				<td>657.75</td>
				<td>NCR, III, IV-A</td>
			</tr>
			<tr>
				<td>4</td>
				<td>Metro Manila Subway Project Phase 1</td>
				<td>Physical Connectivity</td>
				<td>488.48</td>
				<td>NCR</td>
			</tr>
			<tr>
				<td>5</td>
				<td>North Long Haul Railway</td>
				<td>Physical Connectivity</td>
				<td>400.0</td>
				<td>I, II, III</td>
			</tr>
			<tr>
				<td>6</td>
				<td>Daang Maharlika (N1) Improvement</td>
				<td>Physical Connectivity</td>
				<td>251.19</td>
				<td>NCR, I, II, III, IV-A, V, VIII, IX, X, XI, XII, XIII, BARMM</td>
			</tr>
			<tr>
				<td>7</td>
				<td>MRT Line 5</td>
				<td>Physical Connectivity</td>
				<td>250.0</td>
				<td>NCR</td>
			</tr>
			<tr>
				<td>8</td>
				<td>Metro Manila Subway Project - Phase 2</td>
				<td>Physical Connectivity</td>
				<td>247.5</td>
				<td>NCR, III, IV-A</td>
			</tr>
			<tr>
				<td>9</td>
				<td>Bataan-Cavite Interlink Bridge</td>
				<td>Physical Connectivity</td>
				<td>219.31</td>
				<td>III, IV-A</td>
			</tr>
			<tr>
				<td>10</td>
				<td>Panay-Guimaras-Negros Inter-Island Link Bridge</td>
				<td>Physical Connectivity</td>
				<td>187.53</td>
				<td>VI</td>
			</tr>
		</table>
	</div>

	<br>
	<br>

	<div class="row">
		<div class="column">
		  	<p style="text-align:right">The <b>10 most expensive</b> projects are all <span class='highlight'>Physical Connectivity</span> projects, amounting to <span class='highlight'>PHP 4.31101 Trillion</span> in allocated funds.</p>
			<p style="text-align:right"><b>6 out of the 10</b> projects are <b>railway projects</b>,</p>
			<p style="text-align:right">amounting to <span class='highlight'>PHP 2.91735 Trillion</span>.</p>
		</div>
		<div class="column">
		  <img src={pnr} alt="PNR Logo" style="height:20vh">
		  <img src={train} alt="Train" style="height:20vh">
		</div>
	</div> 

	<br>

	<div class="row">
		<div class="column" style="justify-content: right">
			<img src={road} alt="road" style="height:20vh; float:right">
			<img src={airplane} alt="airplane" style="height:20vh; float:right">
		</div>
		<div class="column">
		  	<p style="text-align:left">The second most expensive project is the <b>New Manila International Airport (Bulacan International Airport)</b> at <span class='highlight'>PHP735.63 Billion pesos.</span></p>
			<p style="text-align:left">The remaining three projects are all <b>road related</b>, amounting to <span class='highlight'>PHP 658.03 Billion pesos</span>.</p>
		</div>
	</div>

	<br>
	
	<div class="row">
		<div class="column">
			<br>
		  	<p style="text-align:right"><b>Seven</b> of the most expensive projects include <span class='highlight'>region III</span>, </p>
			<p style="text-align:right">while <b>six</b> include <span class='highlight'>NCR</span>, </p>
			<p style="text-align:right">and <b>five</b> include <span class='highlight'>region IV-A</span>.</p>
		</div>
		<div class="column">
		  <img src={hotspots} alt="hotspots" style="height:30vh">
		</div>
	</div> 

	<br>

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

	<p><i>Note that a single project may be implemented in more than one region, so there is double counting for the values.</i></p>
	<p><i>Additionally each region's count and funds does not include projects that are desginated as 'Nationwide'.</i></p>
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
	p{
		margin: 5px;
	}
	br {
		margin: 3vh 0;
	}

	.row {
	display: flex;
	}

	.column {
		flex: 33.33%;
		padding: 5px;
	}

	.highlight {
		color: #ff3e00;
		font-weight: bold;
	}

</style>
