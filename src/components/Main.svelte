<script>
	import bg from '$lib/assets/header-bg.png';
    import Research from '../components/Research.svelte'
    import Dataset from '../components/Dataset.svelte'
    import EDA from '../components/EDA.svelte'
    import About from '../components/About.svelte'
    import Conclusion from './Conclusion.svelte';
    import Modeling from './Modeling.svelte';
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="relative py-8 sm:py-14 overflow-hidden">
        <!-- Background image -->
        <div class="absolute inset-0 opacity-20 lg:opacity-100 lg:left-[45%]">
            <img src={bg} alt="header-bg" class="w-full h-full object-cover"/>
        </div>
        
        <!-- Content container -->
        <div class="max-w-7xl mx-auto px-4 relative z-10">
            <div class="max-w-[600px]">
                <h2 class="text-2xl leading-relaxed sm:text-3xl sm:leading-relaxed md:text-4xl md:leading-relaxed lg:text-5xl lg:leading-relaxed font-bold">
                    How are <span class="text-yellow-400 boldonse">project funds</span> allocated towards <span class="text-yellow-400 boldonse">sustainability?</span>
                </h2>
                <p class="text-base sm:text-lg md:text-xl mt-6 md:mt-8 lg:mt-10">
                    How does the Philippine government allocate funds for sustainability projects, and what priorities are their current priorities?
                </p>
            </div>
        </div>
    </section>

    <section id="research" class="relative py-16 scroll-mt-24">
        <Research/>
    </section>

    <section id="dataset" class="relative py-16 scroll-mt-24">
        <Dataset/>
    </section>

    <section id="eda" class="relative py-16 scroll-mt-24">
        <EDA/>        
    </section>

    <section id="modeling" class="relative py-16 scroll-mt-24">
        <Modeling></Modeling>
    </section>
    
    <section id="conclusion" class="relative py-16 scroll-mt-24">
        <Conclusion/>
    </section>

    <section id="about-us" class="relative py-16 scroll-mt-24">
        <About/>
    </section>

</main>

<style>
    table {
        border-collapse: collapse;
        width: 100%;
    }
    th, td {
        padding: 0.75rem;
        text-align: left;
        border-bottom: 1px solid rgb(68, 64, 60);
    }
    th {
        background-color: rgba(28, 25, 23, 0.5);
        font-weight: 600;
    }
    tr:hover {
        background-color: rgba(28, 25, 23, 0.3);
    }
</style>