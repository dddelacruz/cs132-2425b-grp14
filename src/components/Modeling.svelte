<script>
    import researchbg from '$lib/assets/research-bg.png';
    import newclark from '$lib/assets/new_clark.png';
    import pampanga from '$lib/assets/pampanga.png';
    import pc_pca from '$lib/assets/pc_pca.png'
    import pc_wordclouds from '$lib/assets/pc_wordclouds.png'
    import npc_pca from '$lib/assets/npc_pca.png'
    import npc_wordclouds from '$lib/assets/npc_wordclouds.png'
</script>
<div>
    <div class="absolute inset-0 opacity-20">
        <img src={researchbg} alt="" class="w-full h-full object-contain bg-no-repeat"/>
    </div>
    
    <div class="max-w-4xl mx-auto px-4 relative z-10">
        <h2 class="text-3xl font-bold mb-12 text-center text-white">Modelling</h2>
        
        <div class="grid grid-cols-1 gap-8">
            <!-- Main Research Question Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">K-Means Clustering</h3>
                <p class="text-gray-100 text-lg mb-6">
                    In order to gather deeper insights into the structure and thematic similarities of infrastructure projects, we applied unsupervised clustering techniques to the dataset. The primary objective was to group projects based on textual and categorical features, particularly the project titles (stop words and common terms like "project" or "plan" were removed), sector, and regions. By doing so, we can uncover patterns and recurring themes that may not be immediately evident through raw data inspection, and we can get a better look at where our national government places their priorities in terms of sustainability projects.
                </p>
                <p class="text-gray-100 text-lg mb-6">
                    We applied K-Means clustering, a method that finds natural groupings in the data without needing predefined categories. Project titles were converted into numerical form using TF-IDF, which highlights important keywords and reduces the impact of common words like “project” or “development.”
                </p>
                <p class="text-gray-100 text-lg mb-6">
                    Due to the sector distribution of the projects, the projects were split into Physical Connectivity and non-Physical Connectivity groups. Each group was then clustered into 4 groups.
                </p>
                <hr class="border-t border-stone-700 mb-4 mt-4"/>
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Physical Connectivity Projects</h3>
                <p class="text-gray-100 text-lg mb-6">
                    Below is a PCA Projection of the Physical Connectivity Projects clusters. As seen in the figure, there is quite a bit of overlap between the clusters. This may be due to the fact that most of the projects in the physical connectivity center have very similar titles. We can see this in the word clouds presented below.
                </p>
                <img src={pc_pca} alt="pca chart" class="w-full max-w-2xl mx-auto mb-4"/>
                <img src={pc_wordclouds} alt="pca wordclouds" class="w-full max-w-2xl mx-auto mb-4"/>
                <ul class="list-disc list-inside">
                    <li class="text-gray-100 text-lg mb-6">
                        <strong>Cluster 0</strong> (7 projects): This cluster deals with networks, rails, and highways—likely representing major corridor or interregional connectivity projects focused on central Mindanao and Metro Manila.
                    </li>
                    <li class="text-gray-100 text-lg mb-6">
                        <strong>Cluster 1</strong> (92 projects): This is the largest cluster, containing many large-scale infrastructure projects such as airports, expressways, bridges, and transit systems—primarily around Metro Manila and major cities.
                    </li>
                    <li class="text-gray-100 text-lg mb-6">
                        <strong>Cluster 2</strong> (24 projects): This group appears to focus on bypasses and coastal roads, especially in Southern Luzon and Mindanao, including key networks in Cagayan de Oro and areas near SLEX.
                    </li>
                    <li class="text-gray-100 text-lg mb-6">
                        <strong>Cluster 3</strong> (14 projects): Projects in this cluster highlight improvement works on existing highways, with repeated mention of Daang Maharlika and regions like Agusan del Norte—suggesting a focus on rehabilitation rather than new builds.
                    </li>
                    </ul>

                    <p class="text-gray-100 text-lg mb-6">
                    While there is some thematic overlap (e.g., many projects involve roads or transport corridors), clustering helped highlight subtle differences in project scale, geographic focus, and type (e.g., new builds vs. improvements).
                    </p>

<h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Non-Physical Connectivity Projects</h3>
                <p class="text-gray-100 text-lg mb-6">
                    Below is a PCA Projection of the Non-Physical Connectivity Projects clusters. Compared to the PCA projection of the Physical Connectivity projects, we see less overlap; likely due to the more varied sectors, regions, and plans with these projects.
                </p>
                <img src={npc_pca} alt="pca chart" class="w-full max-w-2xl mx-auto mb-4"/>
                <img src={npc_wordclouds} alt="pca wordclouds" class="w-full max-w-2xl mx-auto mb-4"/>
                <ul class="list-disc list-inside">
                <li class="text-gray-100 text-lg mb-6">
                    <strong>Cluster 0</strong> (36 projects): This cluster centers on flood control and water infrastructure such as river systems, rural water systems, and national-level flood risk management—especially in Manila and surrounding areas.
                </li>
                <li class="text-gray-100 text-lg mb-6">
                    <strong>Cluster 1</strong> (9 projects): These projects mostly relate to waterway improvements and port infrastructure, with repeated mentions of river channels and specific sites like the Pasig and Marikina Rivers.
                </li>
                <li class="text-gray-100 text-lg mb-6">
                    <strong>Cluster 2</strong> (9 projects): This cluster focuses on irrigation systems, including small reservoir projects in Mindanao and Northern Luzon (e.g., Ilocos Norte) which might likely be agricultural support infrastructure.
                </li>
                <li class="text-gray-100 text-lg mb-6">
                    <strong>Cluster 3</strong> (14 projects): A more mixed category, but largely tied to developments in Clark (e.g., New Clark City) and district hubs that suggest a focus on urban expansion and utility infrastructure. This may be tied to the recent push in urbanizing New Clark City.
                </li>
                </ul>

                <p class="text-gray-100 text-lg mb-6">
                Although most clusters relate to water and infrastructure in some form (since Water Resources is the sector with the most projects after Physical Connectivity), unsupervised clustering helped reveal distinct project focuses: from flood mitigation to agricultural irrigation, port development, and urban expansion. These insights can guide further regional analysis. It even showed the government's possible focus on developing New Clark City.
                </p>
            </div>
        </div>
    </div>
    </div>