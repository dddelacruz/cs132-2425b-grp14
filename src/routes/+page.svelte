<script>
	import Counter from '$lib/Counter.svelte';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="Home Page" content="Home Page" />
</svelte:head>

<section>
	<h1>CS 132 2425B Portfolio</h1>
	<h2>Analyzing the State of Urban and Rural Development Projects in the Philippines in 2024</h2>
	<h2>Group 14 - Sustainability - DE LA CRUZ, MACARAIG, FADRI</h2>
</section>
<hr>

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
	<p><b>Null Hypothesis:</b> There is no significant difference in budget allocation per type of project.</p>
	<p><b>Alternate Hypothesis:</b> There is a significant difference in budget allocation per type of project. </p>

</section>

<hr>

<section>
	<h1>About the Dataset</h1>

	<h2>Description of Data Set</h2>
	<p>The Infrastructure Flagship Projects (IFP) 2024 Dataset, compiled by the National Economic Development Authority (NEDA), provides a comprehensive overview of the status and progress of the national government’s infrastructure initiatives. NEDA aggregates this data yearly to track the status of major government projects. It includes key project details such as title, affected sector, implementing agency, cost and funding allocation, funding source, development partners, geographic coverage, target completion year, and current status at the time of data collection. By analyzing the diverse data points in this dataset, we can gain insights into the government’s priorities regarding sustainability and urban planning.</p>
	
	<h2>Content of Dataset</h2>
	<ul>
		<li>TITLE: Title of the project.</li>
		<li>SECTOR: Sector/focus that would benefit from the project. This includes: Physical Connectivity, Water Resources, Agriculture, etc.</li>
		<li>IMPLEMENTING AGENCY: Government agency responsible for the development of the project. This includes: DPWH, DOTR, DICT, etc.</li>
		<li>INDICATIVE PROJECT COST: The agreed cost of the project.</li>
		<li>FUND SOURCE: Source of the funding of the project. These include: GAA (General Appropriations Act), ODA (Official Development Assistance), PPP, etc.</li>
		<li>DEVELOPMENT PARTNER: External or foreign development partner for the project. This can include support from countries like Japan, China, France, etc., or private companies, like AUB and ADB.</li>
		<li>REGION: Geographical regions covered by the project. This includes: NCR, Region I, Region II, etc.</li>
		<li>TARGET COMPLETION YEAR: Proposed year the project would be completed.</li>
		<li>STATUS/MILESTONE: Current progress/stage of the project. This includes: Completed, Ongoing, Approved for implementation, Under project preparation, etc.</li>
	</ul>

	<h2>Description of Data Collection Process</h2>
	<p>The dataset will be taken from NEDA’s website. The dataset can be found at <a href="https://neda.gov.ph/infrastructure-flagship-projects/?appgw_azwaf_jsc=30n3ZhwmPWnBDkvy6UI96JVnxMXUvCTKIBzDPCFLIjU">[National Economic and Development Authority]</a>.</p>

	<h2>Sampling Method</h2>
	<p>Due to the relatively smaller dataset (186 entries), further reducing the data by extracting samples may exclude certain projects/sectors/regions and may introduce biases. We have decided to study the dataset as is to analyze all relevant data points.</p>

	<h2>Data set size</h2>
	<p>The dataset contains 186 entries, each entry containing the project’s title, affected sector, implementing agency, cost and funding allocation, funding source, development partners, geographic coverage, target completion year, and current status at the time of data collection (9 different values per row).</p>

	<h2>Preprocessing</h2>
	<p>The dataset we took from NEDA has been organized into a readable CSV file, but minimal preprocessing may be required:</p>
		<ul>
			<li>Convert numeric data into float (applicable for INDICATIVE PROJECT COST)</li>
			<li>Simplify categories (like in TARGET COMPLETION YEAR, maybe “beyond 2028” can be 2028+ or converted to int)</li>
			<li>Possible: split rows with multiple categories (like in REGION/S, having “I, IV, NCR” can be split into the individual regions for easier data analysis)</li>
		</ul>
	</section>

<hr>

<br>
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

	section {
		border: 2px solid gray;
  		border-radius: 5px;
		width: 70vw;
		min-width: 500px;
		padding: 25px;
		background-color: rgba(255, 255, 255, 0.8);
		margin: 20px auto;
	}
</style>
