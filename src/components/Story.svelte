<script>
    import researchbg from '$lib/assets/research-bg.png';
    import newclark from '$lib/assets/new_clark.png';
    import pampanga from '$lib/assets/pampanga.png';
    import sdg11 from '$lib/assets/sdg11.jpg';
    import sdg11_2 from '$lib/assets/sdg11_2.png';
</script>
<div>
    <div class="absolute inset-0 opacity-20">
        <img src={researchbg} alt="" class="w-full h-full object-contain bg-no-repeat"/>
    </div>
    
    <div class="max-w-4xl mx-auto px-4 relative z-10">
        <h2 class="text-3xl font-bold mb-12 text-center text-white">Cities for All: A Closer Look at SDG 11 Implementation</h2>
        
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center min-h-[300px]">
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors backdrop-blur-sm h-full">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">What is SDG 11?</h3>
                <p class="text-gray-100 text-lg text-justify">
                    Sustainable Development Goal 11 (SDG 11) aims to <span class="text-yellow-400">“Make Cities and Human Settlements Inclusive, Safe, Resilient, and 
                    Sustainable”</span>. As urban areas are rapidly growing to cater to the increase in population, this Development Goal 
                    addresses how we need to build our cities to be livable and environmentally friendly while also resilient in the face 
                    of climate change and disasters.
                </p>
            </div>
            <div class="h-full">
            <img src={sdg11} alt="SDG 11 Graphic" class="rounded-xl shadow-lg object-cover w-full h-auto" />
            </div>
            
            <div class="h-full">
            <img src={sdg11_2} alt="SDG 11 Graphic_2" class="rounded-xl shadow-lg object-cover w-full h-auto" />
            </div>

            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors backdrop-blur-sm h-full">
        
                <p class="text-gray-100 text-lg text-justify">
                    SDG 11 focuses on a number of key areas regarding urban development such as <span class="text-yellow-400">accessible transport</span>, 
                    <span class="text-yellow-400">disaster risk reduction</span>, and <span class="text-yellow-400">environmental sustainability</span>. It advocates for improvements on air quality, 
                    green spaces and waste management among others in communities that are overlooked. These initiatives are especially vital 
                    for marginalized and underserved communities,
                    which are often overlooked in national development plans. 
                </p>
            </div>
            
        </div>
        <div class="grid grid-cols-1 gap-8 mt-12">

            <!-- Projects of the Philippines Card -->
             <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 backdrop-blur-sm transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Projects of the Philippines</h3>
                <div class="text-gray-100 space-y-4 text-lg">
                    <p class = "text-justify">
                        The Philippines has launched numerous projects and initiatives that align with the goals of SDG 11. Through national planning, projects are led by agencies like the National Economic and Development Authority
                         (NEDA) which aim to improve transportation, housing, disaster risk reduction, and access to basic services. Some notable projects in the different areas of development are shown below
                    </p>
                </div>
            </div>
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 backdrop-blur-sm transition-colors">
                <div class="text-gray-100 space-y-4 text-lg">

                    <p class="font-medium text-yellow-400 text-lg text-center">Housing: New Clark City Affordable Housing</p>
                    <img src={newclark} alt="new clark city" class="w-full h-full object-contain bg-no-repeat"/>
                    <p class = "text-justify">The Bases Conversion and Development Authority plans to collaborate with South Korean companies such as Saekyung Realty Corporation and Overseas Infrastructure and Urban Development Corporation as well as local companies like Sta. Clara International Corporation.</p>
                    <p class = "text-justify">The goal of this project is to create affordable housing in New Clark City, complemented with infrastructure that aligns with SGD 11 such as green spaces, transportation networks and disaster resiliient infrastructure <a class="text-yellow-400 underline hover:text-yellow-300 transition-colors" href = "https://www.dpwh.gov.ph/dpwh/news/35112#:~:text=President%20Ferdinand%20R.,in%20the%20Province%20of%20Pampanga">(Bases Conversion and Development Authority).</a></p>
                    <p class="text-xs">Bases Conversion and Development Authority. (n.d.). BCDA, consortium eye building 61-hectare low-cost housing complex in New Clark City. https://bcda.gov.ph/news/bcda-consortium-eye-building-61-hectare-low-cost-housing-complex-new-clark-city</p>
                </div>
            </div>
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 backdrop-blur-sm transition-colors">
                <div class="text-gray-100 space-y-4 text-lg">
                    <p class="font-medium text-yellow-400 text-lg text-center"> Disaster Risk Reduction integrated disaster risk reduction and climate change adaptation: Pampanga Bay</p>
                    <img src={pampanga} alt="pampanga" class="w-full h-full object-contain bg-no-repeat"/>
                    <p class = "text-justify">Pampanga experiences severe flooding due to a combination of geographical and climate conditions. 
                        First the area is regularly hit by monsoons and typhoons which bring heavy rainfall. Second, Pampanga 
                        is situated on an alluvial plain which makes it prone to flooding because of the limited space for rainwater and 
                        river networks to spread out <a class="text-yellow-400 underline hover:text-yellow-300 transition-colors" href = "https://www.jstage.jst.go.jp/article/jgeography/125/5/125_125.699/_pdf/-char/en">(Naguno and Sawano)</a>. </p>
                    <p class ="text-justify">The Integrated Disaster Risk Reduction and Climate Change Adaptation (IDRR-CCA) Measures in Low Lying Areas of Pampanga Bay is 
                        implemented by the DPWH with funding from the Korean Economic Development and Cooperation Fund (KEDCF), This project 
                        aims to solve the flooding problem in Pampanga by improving the flooding infrastructure such as the drainage system. <a class="text-yellow-400 underline hover:text-yellow-300 transition-colors" href = "https://www.dpwh.gov.ph/dpwh/news/35112#:~:text=President%20Ferdinand%20R.,in%20the%20Province%20of%20Pampanga">(Department of Public Works and Highways)</a></p>
                    <p class="text-xs">Department of Public Works and Highways. (2024, December 9). President Ferdinand R. Marcos Jr. leads inauguration of Pampanga Bypass Road. https://www.dpwh.gov.ph/dpwh/news/35112/ 
                    <p class="text-xs">Nagumo, N., & Sawano, H. (2016). Land classification and flood characteristics of the Pampanga River Basin, Central Luzon, Philippines. Journal of Geography (Chigaku Zasshi), 125(5), 699–716. 
                        https://doi.org/10.5026/jgeography.125.699</p>
                </div>
            </div>

            <!-- Transition Card -->
            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/40 transition-colors">
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Our Motivation</h3>
                <p class="text-gray-100 text-lg text-justify">
                    While these initiatives demonstrate how the projects of the Philippines align with the goals of SDG 11, they also expose a pattern: these projects are mostly centered around Metro Manila. 
                    The lack of regional focus begs the question – are other communities being left behind in terms of national planning and infrastructure development?
                </p>
                <br>
                <p class="text-gray-100 text-lg text-justify">
                    In light of this pattern, we set out to investigate the national projects for sustainability. Understanding what the projects are about, how it is implemented and 
                    how resources are allocated among them offers us insights about the governments priorities.
                    By doing so, we can uncover if these developmental efforts are inclusive of different communities,
                    and if it solves our unique challenges.
                </p>
            </div>

            
           
        </div>
    </div>
    </div>