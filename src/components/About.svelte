<script>
    import datasetbg from '$lib/assets/dataset-bg.png';
    import delacruz from '$lib/assets/avatar_delacruz.png'
    import fadri from '$lib/assets/avatar_fadri.png'
    import macaraig from '$lib/assets/avatar_macaraig.jpg';
</script>

<div>
    <div class="absolute inset-0 opacity-20">
        <img src={datasetbg} alt="" class="w-full h-full object-contain bg-no-repeat"/>
    </div>
    
    <div class="max-w-6xl mx-auto px-4 relative z-10">
        <h2 class="text-3xl font-bold mb-12 text-center text-white">About Us</h2>
        
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">

            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 backdrop-blur-sm transition-colors">
                <img src={delacruz} alt="d delacruz" class="object-contain bg-no-repeat rounded-full mx-auto w-24 h-24 mb-4"/>
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Diana Mae D. de la Cruz</h3>
                <hr class="border-t border-stone-700 mb-4"/>
                <div class="text-gray-100 space-y-4 text-lg text-center">
                    <p>Currently a graduating 4th year BS Computer Science student under the Scientific Computing Laboratory. Usually found playing maimai.</p>
                </div>
                <hr class="border-t border-stone-700 mb-4 mt-4"/>
                <a href="https://github.com/dddelacruz" class="text-yellow-400 hover:text-yellow-300 transition-colors hover:underline text-center block">Github link </a>
            </div>

            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 backdrop-blur-sm transition-colors">
                <img src={fadri} alt="vincent fadri" class="object-contain bg-no-repeat rounded-full mx-auto w-24 h-24 mb-4"/>
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Vincent Paul C. Fadri</h3>
                <hr class="border-t border-stone-700 mb-4"/>
                <div class="text-gray-100 space-y-4 text-lg text-center">
                    <p>4th year BS Computer Science Student:)</p>
                </div>
                <hr class="border-t border-stone-700 mb-4 mt-4"/>
                <a href="https://github.com/vpcfadri1" class="text-yellow-400 hover:text-yellow-300 transition-colors hover:underline text-center block">Github link </a>
            </div>

            <div class="bg-stone-800/30 rounded-lg border border-stone-700 p-6 hover:bg-stone-800/50 backdrop-blur-sm transition-colors">
                <img src={macaraig} alt="manuel macaraig" class="object-contain bg-no-repeat rounded-full mx-auto w-24 h-24 mb-4"/>
                <h3 class="text-2xl font-semibold mb-4 text-yellow-400 text-center">Manuel Macaraig</h3>
                <hr class="border-t border-stone-700 mb-4"/>
                <div class="text-gray-100 space-y-4 text-lg text-center">
                    <p>Currently a graduating 4th year BS Computer Science student. If he's not coding, he's either making beats or cool posters :] </p>
                </div>
                <hr class="border-t border-stone-700 mb-4 mt-4"/>
                <a href="https://github.com/mdmacaraig" class="text-yellow-400 hover:text-yellow-300 transition-colors hover:underline text-center block">Github link </a>
            </div>

            

        </div>
    </div>
</div>