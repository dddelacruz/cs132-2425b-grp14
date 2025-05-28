<script>
    import datasetbg from '$lib/assets/dataset-bg.png';
</script>

<div>
    <div class="absolute inset-0 opacity-20">
        <img src={datasetbg} alt="" class="w-full h-full object-contain bg-no-repeat"/>
    </div>
    
    <div class="max-w-4xl mx-auto px-4 relative z-10">
        <h2 class="text-3xl font-bold mb-12 text-center text-white">Dataset</h2>
        
        <div class="grid grid-cols-1 gap-8">
            <!-- Description Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Description</h3>
                <p class="text-gray-100 text-lg">
                    The Infrastructure Flagship Projects (IFP) 2024 Dataset, compiled by the National Economic Development Authority (NEDA), provides a comprehensive overview of the status and progress of the national government's infrastructure initiatives. NEDA aggregates this data yearly to track the status of major government projects. It includes key project details such as title, affected sector, implementing agency, cost and funding allocation, funding source, development partners, geographic coverage, target completion year, and current status at the time of data collection. By analyzing the diverse data points in this dataset, we can gain insights into the government's priorities regarding sustainability and urban planning.
                </p>
            </div>

            <!-- Background Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 backdrop-blur-sm transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Content</h3>
                <div class="text-gray-100 space-y-4 text-lg">
                    <ul class="list-disc list-inside pl-4 space-y-2">
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
                </div>
            </div>

            <!-- Research Problems Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Data Collection</h3>
                <div class="text-gray-100 space-y-4">
                    <div>
                        <p class="pl-4 text-gray-200 text-lg">The dataset will be taken from NEDA's IFPs. The dataset can be found at <a class="text-yellow-400 hover:underline" href="https://depdev.gov.ph/infrastructure-flagship-projects/">their website.</a></p>
                        <br>
                        <hr class="opacity-20">
                        <br>
                        <p class="font-medium text-yellow-400 text-lg">Sampling Method</p>
                        <p class="pl-4 text-gray-200 text-lg">Due to the relatively smaller dataset (186 entries), further reducing the data by extracting samples may exclude certain projects/sectors/regions and may introduce biases. We have decided to study the dataset as is to analyze all relevant data points.</p>
                    </div>
                    <div>
                        <p class="font-medium text-yellow-400 text-lg">Dataset Size</p>
                        <p class="pl-4 text-gray-200 text-lg">Investigate how funds are distributed between different sustainability projects</p>
                    </div>
                    <div>
                        <p class="font-medium text-yellow-400 text-lg">Preprocessing</p>
                        <p class="pl-4 text-gray-200 text-lg">Investigate the distribution of funds according to location</p>
                    </div>
                </div>
            </div>

            <!-- Hypotheses Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400">Hypotheses</h3>
                <div class="text-gray-100 space-y-4">
                    <div>
                        <p class="font-medium text-yellow-400 text-lg">Null Hypothesis:</p>
                        <p class="pl-4 text-gray-200 text-lg">There is no significant difference in budget allocation per type of project.</p>
                    </div>
                    <div>
                        <p class="font-medium text-yellow-400 text-lg">Alternate Hypothesis:</p>
                        <p class="pl-4 text-gray-200 text-lg">There is a significant difference in budget allocation per type of project.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>