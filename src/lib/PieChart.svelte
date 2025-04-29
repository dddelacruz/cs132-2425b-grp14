<script>
    // original: https://observablehq.com/@d3/pie-chart/2
	// svelte version: Sebastian Lammers https://vis.social/@seblammers
	
	import * as d3 from "d3";
	
	// Receive plot data as prop.
    export let data;
	
	// Specify the chart’s dimensions.
    const width = 928;
    const height = 250;

    // Create the color scale.
    const colourScale = d3.scaleOrdinal()
		.domain(data.map(d => d.name))
		.range(d3.quantize(t => d3.interpolateSpectral(t * 0.8 + 0.1), data.length).reverse())

    // Create the pie layout and arc generator.
    const pie = d3.pie()
		.sort(null)
		.value(d => d.value);

    const arcPath = d3.arc()
		// control the style of the pie slices;
		// try changing the inner radius to 100 to see what happens
		.innerRadius(75)
		.outerRadius(Math.min(width, height) / 2 - 1);

  const labelRadius = arcPath.outerRadius()() * 0.8;

  // A separate arc generator for labels.
  const arcLabel = d3.arc()
		.innerRadius(labelRadius)
		.outerRadius(labelRadius);

  const arcs = pie(data);
</script>

<svg
  {width}
  {height}
  viewBox="{-width / 2}, {-height / 2}, {width}, {height}"
  style:max-width="100%"
  style:height="auto"
>

	<g class="data">

		<!-- Loop through the data-slices. -->
		{#each arcs as slice}
			
			<!-- Add each pie-slice. -->
			<path 
				d={arcPath(slice)}
				fill={colourScale(slice.data.name)}
				stroke="white"
				/>

			<!-- Add each label. -->
			<text
				style="font-weight: bold"
				transform="translate({arcLabel.centroid(slice)})"
				text-anchor="middle"
				>
				{slice.data.name}
			</text>
			
			<!-- show the value if there is enough room. -->
			{#if (slice.endAngle - slice.startAngle) > 0.25}
				<text
					text-anchor="middle"
					transform="translate({[arcLabel.centroid(slice)[0], arcLabel.centroid(slice)[1] + 10]})"
					>
					{slice.data.value.toLocaleString("en-US")}
				</text>
			{/if}
		{/each}
	</g>
</svg>

<aside>
	<p><strong>Use Pie Charts responsibly.</strong><br>
	See <a 
				href="https://academy.datawrapper.de/article/127-what-to-consider-when-creating-a-pie-chart" 
				target="_blank"
				rel="noopener noreferrer"
			>this article</a>
		for advice on when and how to best use pie charts.<br>
		(This example chart is <i>not</i> a good use of a pie chart...)
	</p>
	

</aside>
<style>
	svg {
		font-size: 10px;
	}
	aside {
		text-align: center;
	}
</style>
