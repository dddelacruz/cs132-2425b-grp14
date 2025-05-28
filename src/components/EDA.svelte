<script>
    import datasetbg from '$lib/assets/dataset-bg.png';
    import pie_chart from '$lib/assets/pie_chart.png';
	import bar_project_count from '$lib/assets/bar_project_count.png';
	import bar_region_count from '$lib/assets/bar_region_count_stacked2.png';
	import bar_region_funds from '$lib/assets/bar_region_funds_stacked2.png';
	import pnr from '$lib/assets/pnr.png';
	import train from '$lib/assets/train.png';
	import airplane from '$lib/assets/airplane.png';
	import road from '$lib/assets/road.png';
	import hotspots from '$lib/assets/hotspots.png';
	import Hypothesis_1 from '$lib/assets/Hypothesis_1.png';
	import Hypothesis_2 from '$lib/assets/Hypothesis_2.png';
	import Hypothesis_3 from '$lib/assets/Hypothesis_3.png';
	import Hypothesis_4 from '$lib/assets/Hypothesis_4.png';
	import nutshell from '$lib/assets/nutshell_plot.png'
</script>
<div>
    <!-- Background image -->
    <div class="absolute inset-0 opacity-20">
        <img src={datasetbg} alt="" class="w-full h-full object-contain bg-no-repeat"/>
    </div>
    
    <div class="max-w-4xl mx-auto px-4 relative z-10">
        <h2 class="text-3xl font-bold mb-12 text-center text-white">Exploratory Data Analysis</h2>
        
        <!-- Nutshell Plot Section -->
        <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 transition-colors mb-8">
            <h3 class="text-2xl font-semibold mb-6 text-yellow-400 text-center">Project Distribution Overview</h3>
            <div class="flex flex-col items-center">
                <img alt="Nutshell Plot" src={nutshell} class="w-full max-w-3xl mb-6"/>
                <p class="text-gray-100 text-lg text-justify">
                    This choropleth map shows the distribution of sustainability projects per region around the Philippines. It can be seen that the majority of projects are concentrated around Region III, IV-A, and NCR. This can mainly be attributed to those regions being part of three large projects: the North-South Commuter Railway, the Bulacan International Airport, and Subic-Clark-Manila-Batangas Dedicated Rail Corridor. Furthermore, most of the projects regarding sustainability are classified as "Physical Connectivity" projects, in other words: projects regarding transportation and connectivity of locations. There are around four times more Physical Connectivity projects compared to Water Resources projects, which is the second most common type. There appears to be an inequality in the number of projects per project type along with per region.
                </p>
            </div>
            <div class="mt-8 w-full invert">
                <iframe title='Nutshell Plot' src="/nutshell_plot.htm" class="w-full h-[800px] border-none"></iframe>
            </div>
        </div>

        <!-- Project Graphs Section -->
        <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 transition-colors mb-8">
            <h3 class="text-2xl font-semibold mb-6 text-yellow-400 text-center">Project Fund Allocation Analysis</h3>
            
            <div class="mb-8">
                <h4 class="text-xl font-semibold mb-4 text-yellow-400">1. How are project funds allocated towards sustainability?</h4>
                <div class="bg-stone-900/50 rounded-lg p-4 mb-6">
                    <p class="text-gray-100 text-lg">Total amount of funds allocated: <span class="text-yellow-400 font-semibold">PHP 9.5684 Trillion</span></p>
                </div>

                <!-- Pie Chart -->
                <div class="flex flex-col items-center mb-8">
                    <p class="text-gray-100 text-lg font-semibold mb-4">Percentage of funds allocated to each sector</p>
                    <img alt="Pie Chart per Sector" src={pie_chart} class="w-full max-w-3xl invert"/>
                </div>

                <!-- Fund Allocation Table -->
                <div class="overflow-x-auto">
                    <table class="w-full text-gray-100">
                        <thead class="bg-stone-900/50">
                            <tr>
                                <th class="p-3 text-left">Sector</th>
                                <th class="p-3 text-right">Indicative Project Cost (in Php B)</th>
                                <th class="p-3 text-right">%</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">8,343.71</td>
                                <td class="p-3 text-right">87.20</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">Water Resources</td>
                                <td class="p-3 text-right">775.07</td>
                                <td class="p-3 text-right">8.10</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">Agriculture</td>
                                <td class="p-3 text-right">213.68</td>
                                <td class="p-3 text-right">2.23</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">Health</td>
                                <td class="p-3 text-right">95.73</td>
                                <td class="p-3 text-right">1.00</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">Digital Connectivity</td>
                                <td class="p-3 text-right">78.11</td>
                                <td class="p-3 text-right">0.82</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">Education</td>
                                <td class="p-3 text-right">30.56</td>
                                <td class="p-3 text-right">0.32</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">Other Infrastructure</td>
                                <td class="p-3 text-right">21.34</td>
                                <td class="p-3 text-right">0.22</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">Power and Energy</td>
                                <td class="p-3 text-right">10.19</td>
                                <td class="p-3 text-right">0.10</td>
                            </tr>
                            <tr class="border-b border-stone-700 font-semibold bg-stone-900/30">
                                <td class="p-3">TOTAL</td>
                                <td class="p-3 text-right">95,684</td>
                                <td class="p-3 text-right">100</td>
                            </tr>
                        </tbody>
                    </table>
                </div>

                <div class="bg-stone-900/50 rounded-lg p-4 mt-8 mb-6">
                    <p class="text-gray-100 text-lg mb-2">It can be seen that the sector that is most invested on is <span class="text-yellow-400 font-semibold">Physical Connectivity</span>, with the majority of funds allocated going towards it.</p>
                    <p class="text-gray-100 text-lg">Investigating further to see the ten most expensive projects:</p>
                </div>

                <!-- Top 10 Projects Table -->
                <div class="overflow-x-auto mt-6">
                    <p class="text-gray-100 text-lg font-semibold mb-4">Table containing the ten most expensive projects</p>
                    <table class="w-full text-gray-100">
                        <thead class="bg-stone-900/50">
                            <tr>
                                <th class="p-3 text-left">Rank</th>
                                <th class="p-3 text-left">Project Title</th>
                                <th class="p-3 text-left">Sector</th>
                                <th class="p-3 text-right">Indicative Project Cost (in Php B)</th>
                                <th class="p-3 text-left">Region/s</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">1</td>
                                <td class="p-3">North-South Commuter Railway (PNR North 1,PNR North 2,PNR South Commuter)</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">873.62</td>
                                <td class="p-3">NCR, III, IV-A</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">2</td>
                                <td class="p-3">New Manila International Airport (Bulacan International Airport)</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">735.63</td>
                                <td class="p-3">III</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">3</td>
                                <td class="p-3">Subic-Clark-Manila-Batangas Dedicated Rail Corridor</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">657.75</td>
                                <td class="p-3">NCR, III, IV-A</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">4</td>
                                <td class="p-3">Metro Manila Subway Project Phase 1</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">488.48</td>
                                <td class="p-3">NCR</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">5</td>
                                <td class="p-3">North Long Haul Railway</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">400.00</td>
                                <td class="p-3">I, II, III</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">6</td>
                                <td class="p-3">Daang Maharlika (N1) Improvement</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">251.19</td>
                                <td class="p-3">NCR, I, II, III, IV-A, V, VIII, IX, X, XI, XII, XIII, BARMM</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">7</td>
                                <td class="p-3">MRT Line 5</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">250.00</td>
                                <td class="p-3">NCR</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">8</td>
                                <td class="p-3">Metro Manila Subway Project - Phase 2</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">247.50</td>
                                <td class="p-3">NCR, III, IV-A</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">9</td>
                                <td class="p-3">Bataan-Cavite Interlink Bridge</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">219.31</td>
                                <td class="p-3">III, IV-A</td>
                            </tr>
                            <tr class="border-b border-stone-700">
                                <td class="p-3">10</td>
                                <td class="p-3">Panay-Guimaras-Negros Inter-Island Link Bridge</td>
                                <td class="p-3">Physical Connectivity</td>
                                <td class="p-3 text-right">187.53</td>
                                <td class="p-3">VI</td>
                            </tr>
                        </tbody>
                    </table>
                </div>

                <!-- Railway Projects Summary -->
                <div class="flex flex-col md:flex-row gap-8 mt-8 bg-stone-900/30 rounded-lg p-6">
                    <div class="flex-1">
                        <div class="text-right">
                            <p class="text-gray-100 text-lg mb-2">The <span class="text-yellow-400 font-semibold">10 most expensive</span> projects are all <span class="text-yellow-400 font-semibold">Physical Connectivity</span> projects, amounting to <span class="text-yellow-400 font-semibold">PHP 4.31101 Trillion</span> in allocated funds.</p>
                            <p class="text-gray-100 text-lg mb-2"><span class="font-semibold">6 out of the 10</span> projects are <span class="font-semibold">railway projects</span>,</p>
                            <p class="text-gray-100 text-lg">amounting to <span class="text-yellow-400 font-semibold">PHP 2.91735 Trillion</span>.</p>
                        </div>
                    </div>
                    <div class="flex gap-4 justify-center items-center md:w-1/3">
                        <img src={pnr} alt="PNR Logo" class="h-32"/>
                        <img src={train} alt="Train" class="h-32 invert"/>
                    </div>
                </div>

                <!-- Airport and Roads Summary -->
                <div class="flex flex-col md:flex-row gap-8 mt-8 bg-stone-900/30 rounded-lg p-6">
                    <div class="flex gap-4 justify-center items-center md:w-1/3 order-2 md:order-1">
                        <img src={road} alt="road" class="h-32"/>
                        <img src={airplane} alt="airplane" class="h-32 invert"/>
                    </div>
                    <div class="flex-1 order-1 md:order-2">
                        <div class="text-left">
                            <p class="text-gray-100 text-lg mb-2">The second most expensive project is the <span class="font-semibold">New Manila International Airport (Bulacan International Airport)</span> at <span class="text-yellow-400 font-semibold">PHP735.63 Billion pesos.</span></p>
                            <p class="text-gray-100 text-lg">The remaining three projects are all <span class="font-semibold">road related</span>, amounting to <span class="text-yellow-400 font-semibold">PHP 658.03 Billion pesos</span>.</p>
                        </div>
                    </div>
                </div>

                <!-- Regional Distribution Summary -->
                <div class="flex flex-col md:flex-row gap-8 mt-8 bg-stone-900/30 rounded-lg p-6">
                    <div class="flex-1">
                        <div class="text-right">
                            <p class="text-gray-100 text-lg mb-2"><span class="font-semibold">Seven</span> of the most expensive projects include <span class="text-yellow-400 font-semibold">region III</span>,</p>
                            <p class="text-gray-100 text-lg mb-2">while <span class="font-semibold">six</span> include <span class="text-yellow-400 font-semibold">NCR</span>,</p>
                            <p class="text-gray-100 text-lg">and <span class="font-semibold">five</span> include <span class="text-yellow-400 font-semibold">region IV-A</span>.</p>
                        </div>
                    </div>
                    <div class="flex justify-center items-center md:w-1/2">
                        <img src={hotspots} alt="hotspots" class="h-64 invert"/>
                    </div>
                </div>
            </div>
        </div>

        <!-- Hypothesis Testing Section -->
        <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 transition-colors">
            <h3 class="text-2xl font-semibold mb-6 text-yellow-400 text-center">Hypothesis Testing</h3>
            
            <div class="text-gray-100 text-lg mb-8 bg-stone-900/30 rounded-lg p-6">
                <p class = "text-justify">The hypothesis testing applies chi-square goodness-of-fit test and the Kolmogorov-Smirnov test to evaluate whether the actual allocation of projects and project funds
                in the Philippines aligns with an equal distribution or a distribution based on the regional population. Through these tests, we will see if the government 
                prioritizes each region equally with each project.</p>
            </div>

            <h4 class="text-xl font-semibold mb-4 text-yellow-400">Projects by Count</h4>
            <div class="text-gray-100 text-lg mb-8 bg-stone-900/30 rounded-lg p-6">
                <p class = "text-justify">
                We will be using the <span class="font-semibold">chi-square goodness-of-fit</span> to check whether the allocation of projects between each region is uniform or if it follows
                the population distribution across regions. Doing this helps us assess if resources are being distributed fairly across regions. 
                The categorical data would be the region, and each project was divided based on the number of regions affected to make them <span class="font-semibold">mutually exclusive</span>.
                The expected number of projects per region is either equal or according to the population which is significantly large (5 or more).
                </p>
            </div>

            <!-- Test Results 1 -->
            <div class="bg-stone-900/30 rounded-lg p-6 mb-8">
                <img src={Hypothesis_1} alt="Hypothesis Test 1" class="w-full max-w-3xl mx-auto mb-4"/>
                <p class="text-gray-100 text-lg mb-2">A Chi-Square Goodness of Fit test will be used for the hypothesis testing at a 95% confidence interval</p>
                <p class="text-gray-100 text-lg mb-2">Chi-square test statistic: <span class="text-yellow-400 font-semibold">105.337</span>, p-value: <span class="text-yellow-400 font-semibold">9.035e-15</span></p>
                <p class="text-gray-100 text-lg mb-4">Since p &lt; 0.05, <span class="font-semibold">we reject the null hypothesis</span></p>
                <hr class="border-stone-700 my-4"/>
                <p class="text-gray-100 text-lg font-semibold">Sustainability projects are not evenly distributed among regions in the Philippines</p>
            </div>

            <!-- Test Results 2 -->
            <div class="bg-stone-900/30 rounded-lg p-6 mb-8">
                <img src={Hypothesis_2} alt="Hypothesis Test 2" class="w-full max-w-3xl mx-auto mb-4"/>
                <p class="text-gray-100 text-lg mb-2">A Chi-Square Goodness of Fit test will be used for the hypothesis testing at a 95% confidence interval</p>
                <p class="text-gray-100 text-lg mb-2">Chi-square test statistic is: <span class="text-yellow-400 font-semibold">31.593</span>, p-value: <span class="text-yellow-400 font-semibold">0.011</span></p>
                <p class="text-gray-100 text-lg mb-4">Since p &lt; 0.05, <span class="font-semibold">we reject the null hypothesis</span></p>
                <hr class="border-stone-700 my-4"/>
                <p class="text-gray-100 text-lg font-semibold">Sustainability projects are not distributed proportionally to the population of each region as a fraction of the total population.</p>
            </div>

            <h4 class="text-xl font-semibold mb-4 text-yellow-400">Projects by Funding</h4>
            <div class="text-gray-100 text-lg mb-8 bg-stone-900/30 rounded-lg p-6">
                <p class = "text-justify">
                We will be using the <span class="font-semibold">chi-square goodness-of-fit</span> to check whether the fund allocation of projects between each region is uniform or if it follows
                the population distribution across regions. Again, doing this helps us assess if resources are being distributed fairly across regions. 
                The categorical data would be the region, and each project's fund was divided based on the number of regions affected to make them <span class="font-semibold">mutually exclusive</span>.
                We will treat each project fund similar to the count in the previous test. We think that the chi-square goodness of fit is more suitable because
                regions are treated as categories and a test like Kolmogorov-Smirnov is designed for continuous distributions and would be less appropriate, as it focuses on comparing 
                cumulative distribution functions rather than categorical proportions.
                </p>
            </div>

            <!-- Test Results 3 -->
            <div class="bg-stone-900/30 rounded-lg p-6 mb-8">
                <img src={Hypothesis_3} alt="Hypothesis Test 3" class="w-full max-w-3xl mx-auto mb-4"/>
                <p class="text-gray-100 text-lg mb-2">A Chi-Square Goodness of Fit test will be used for the hypothesis testing at a 95% confidence interval</p>
                <p class="text-gray-100 text-lg mb-2">Chi-square test statistic is: <span class="text-yellow-400 font-semibold">14926.666</span>, p-value: <span class="text-yellow-400 font-semibold">0.0</span></p>
                <p class="text-gray-100 text-lg mb-4">Since p &lt; 0.05, <span class="font-semibold">we reject the null hypothesis</span></p>
                <hr class="border-stone-700 my-4"/>
                <p class="text-gray-100 text-lg font-semibold">The funding of Sustainability projects are not evenly distributed among regions in the Philippines</p>
            </div>

            <!-- Test Results 4 -->
            <div class="bg-stone-900/30 rounded-lg p-6 mb-8">
                <img src={Hypothesis_4} alt="Hypothesis Test 4" class="w-full max-w-3xl mx-auto mb-4"/>
                <p class="text-gray-100 text-lg mb-2">A Chi-Square Goodness of Fit test will be used for the hypothesis testing at a 95% confidence interval</p>
                <p class="text-gray-100 text-lg mb-2">Chi-square test statistic is: <span class="text-yellow-400 font-semibold">3723.782</span>, p-value: <span class="text-yellow-400 font-semibold">0.0</span></p>
                <p class="text-gray-100 text-lg mb-4">Since p &lt; 0.05, <span class="font-semibold">we reject the null hypothesis</span></p>
                <hr class="border-stone-700 my-4"/>
                <p class="text-gray-100 text-lg font-semibold">The funding of Sustainability projects are not distributed proportionally to the population of each region as a fraction of the total population.</p>
            </div>

            <h4 class="text-xl font-semibold mb-4 text-yellow-400">Hypothesis Conclusion</h4>
            <div class="text-gray-100 text-lg bg-stone-900/30 rounded-lg p-6">
                <p class = "text-justify">
                We can see that from the different Hypothesis tests, the allocation of project resources is not aligned with the uniform distribution or the 
                population based distribution. The resource distribution is uneven and policy adjustments may be warranted to ensure equitable allocation across
                regions. Additionally, the different graphs and plots show us that the projects are concentrated in Luzon, specifically NCR which reflects a more 
                centralized approach to development.
                </p>
            </div>
        </div>

        <br>

        <!-- EDA Discussion Section -->
        <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 transition-colors mb-8">
            <h3 class="text-2xl font-semibold mb-6 text-yellow-400 text-center">EDA Discussion</h3>
            <div class="flex flex-col items-center text-justify">
                <p class="text-gray-100 text-lg mb-5">
                    It can be seen from the EDA conducted, that a majority of the sustainability projects listed in the 2024 IFP Dataset are physical connectivity projects, mainly concerning transportation and roads. Furthermore, a majority of the funds and projects are concentrated in the central Luzon area including Regions III, IV-A, and NCR. 
                </p>
                <p class="text-gray-100 text-lg mb-5">
                    The top ten most expensive projects are all Physical Connectivity projects. The most expensive project, at Php 873.62, is the North-South Commuter Railway in regions III, IV-A, and NCR. The second most expensive is the New Manila International Airport (Bulacan International Airport) at Php 735.63 for region III. 
                </p>
                <p class="text-gray-100 text-lg mb-5">
                    Of the ten most expensive projects, six of them are railway projects at PHP 2.917 Trillion total, three are road projects at PHP 658.03 Billion, and the last one is an airport project at Php 735.63. Seven of the most expensive projects include region III, while six include NCR, and five include region IV-A.
                </p>
                <p class="text-gray-100 text-lg mb-5">
                    Furthermore, Physical Connectivity projects amount to 87.20% of the funds allocated, with the the second most funded being Water Resources only amounting to 8.10% of the budget, and the third most funded being Agriculture at only 2.23% of the budget. 
                </p>
                <p class="text-gray-100 text-lg mb-5">
                    Based on the results from the dataset, it can be seen that the government mostly prioritizes Physical Connectivity projects, with a focus on Regions III, IV-A, and NCR. 
                </p>
                <p class="text-gray-100 text-lg mb-5">
                    Despite these results, it is not truly enough to draw a definitive conclusion on what the government is really prioritizing. The top ten most expensive projects mentioned are all major development projects that are mostly in the foundational and construction stages. The data for the funding does not take into account the timeline of each project, nor their current status. Additionally, each project has different implementing agencies, funding sources, and development partners, which were not taken into account for this study. These factors can be further investigated in order to give a more complete picture. Another possible avenue for further study is the analysis and comparison of projects within project types or within regions. 
                </p>
            </div>
        </div>
    </div>
</div>