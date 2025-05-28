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
                <div class="text-gray-100 space-y-4 text-lg text-justify">
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
             

            <!-- Transition Card -->
            

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