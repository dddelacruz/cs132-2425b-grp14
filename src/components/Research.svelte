<script>
    import researchbg from '$lib/assets/research-bg.png';
    import newclark from '$lib/assets/new_clark.png';
    import pampanga from '$lib/assets/pampanga.png';
</script>
<div>
    <div class="absolute inset-0 opacity-20">
        <img src={researchbg} alt="" class="w-full h-full object-contain bg-no-repeat"/>
    </div>
    
    <div class="max-w-4xl mx-auto px-4 relative z-10">
        <h2 class="text-3xl font-bold mb-12 text-center text-white">Research Design</h2>
        
        <div class="grid grid-cols-1 gap-8">
            <!-- Main Research Question Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">We wanted to ask...</h3>
                <p class="text-gray-100 text-lg">
                    How does the Philippine government allocate funds for sustainability projects, and what priorities are their current priorities?
                </p>
            </div>

            <!-- Background Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 backdrop-blur-sm transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Background of the Study</h3>
                <div class="text-gray-100 space-y-4 text-lg">
                    <p>
                        SDG 11 goal is to "Make Cities and Human Settlements Inclusive, Safe, Resilient, and Sustainable". According to the United Nations, this SDG tackles problems related to transport, housing, and sustainable development such as Disaster Risk Reduction, accessibility, and minimization of environmental impact.
                    </p>
                    <p>
                        Key performance indicators are used to quantify the SDG and according to the SDG watch released by the Philippine Statistics Authority, the Philippines is far from reaching the desired goals for 2023. These indicators include:
                    </p>
                    <ul class="list-disc list-inside pl-4 space-y-2">
                        <li>11.1.1p1: Proportion of urban population who are informal settlers</li>
                        <li>11.5.1: Number of deaths, missing persons and directly affected persons attributed to disasters per 100,000 population</li>
                        <li>11.6.2.p1: Percentage of highly urbanized and other major urban centers within ambient air quality guidelines value increased</li>
                    </ul>
                    <p>
                        This study uses a dataset from NEDA which contains the state current and future projects of the Philippines to investigate the different projects being implemented by the government.
                    </p>
                </div>
            </div>

            <!-- Projects of the Philippines Card -->
             <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 backdrop-blur-sm transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Projects of the Philippine</h3>
                <div class="text-gray-100 space-y-4 text-lg">
                    <p>
                        The Philippines has launched numerous projects and initiatives that align with the goals of SDG 11. Through national planning, projects are led by agencies like the National Economic and Development Authority (NEDA) which aim to improve transportation, housing, disaster risk reduction, and access to basic services.
                    </p>
                    <p>
                        Some notable projects in the different areas of development are:
                    </p>

                    <p class="font-medium text-yellow-400 text-lg">1. Housing: New Clark City Affordable Housing</p>
                    <img src={newclark} alt="new clark city" class="w-full max-w-3xl mx-auto mb-4"/>
                    <p>The Bases Conversion and Development Authority plans to collaborate with South Korean companies such as Saekyung Realty Corporation and Overseas Infrastructure and Urban Development Corporation as well as local companies like Sta. Clara International Corporation.</p>
                    <p>The goal of this project is to create affordable housing in New Clark City, complemented with infrastructure that aligns with SGD 11 such as green spaces, transportation networks and disaster resiliient infrastructure.</p>
                    <p class="text-xs">https://bcda.gov.ph/news/bcda-consortium-eye-building-61-hectare-low-cost-housing-complex-new-clark-city</p>
                
                    <p class="font-medium text-yellow-400 text-lg">2. Disaster Risk Reduction integrated disaster risk reduction and climate change adaptation: Pampanga Bay</p>
                    <img src={pampanga} alt="pampanga" class="w-full max-w-3xl mx-auto mb-4"/>
                    <p>Pampanga experiences severe flooding due to a combination of geographical and climate conditions. First the area is regularly hit by monsoons and typhoons which bring heavy rainfall. Second, Pampanga is situated on an alluvial plain which makes it prone to flooding because of the limited space for rainwater and river networks to spread out. </p>
                    <p>The Integrated Disaster Risk Reduction and Climate Change Adaptation (IDRR-CCA) Measures in Low Lying Areas of Pampanga Bay is implemented by the DPWH with funding from the Korean Economic Development and Cooperation Fund (KEDCF), This project aims to solve the flooding problem in Pampanga by improving the flooding infrastructure such as the drainage system.</p>
                    <p class="text-xs break-words">https://www.dpwh.gov.ph/dpwh/news/35112#:~:text=President%20Ferdinand%20R.,in%20the%20Province%20of%20Pampanga</p>
                </div>
            </div>

            <!-- Transition Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Our Motivation</h3>
                <p class="text-gray-100 text-lg">
                    While these initiatives demonstrate how the projects of the Philippines align with the goals of SDG 11, they also expose a pattern: these projects are mostly centered around Metro Manila. The lack of regional focus begs the question – are other communities being left behind in terms of national planning and infrastructure development?
                </p>
                <br>
                <p class="text-gray-100 text-lg">
                    This question has prompted the team to investigate the current projects of the Philippines. By doing this research, we will be able to find patterns about national investment as well as opportunities to pursue the SDG 11 with no community left behind.
                </p>
            </div>

            <!-- Research Problems Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400">Research Problems</h3>
                <div class="text-gray-100 space-y-4">
                    <div>
                        <p class="font-medium text-yellow-400 text-lg">1. How are project funds allocated towards sustainability?</p>
                        <p class="pl-4 text-gray-200 text-lg">Investigate how funds are distributed between sustainability projects as opposed to other projects</p>
                    </div>
                    <div>
                        <p class="font-medium text-yellow-400 text-lg">2. What kind of sustainability projects is the current government focused on?</p>
                        <p class="pl-4 text-gray-200 text-lg">Investigate how funds are distributed between different sustainability projects</p>
                    </div>
                    <div>
                        <p class="font-medium text-yellow-400 text-lg">3. Which sectors/regions does the government prioritize?</p>
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