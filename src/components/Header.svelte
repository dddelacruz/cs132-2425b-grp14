<script>
    export let y;
    let tabs = [
        {name: 'Research', link: '#research'},
        {name: 'Dataset', link: '#dataset'},
        {name: 'EDA', link: '#eda'},
        {name: 'Modeling', link: '#modeling'},
        {name: 'Conclusion', link: '#conclusion'},
        {name: 'About Us', link: '#about-us'},
    ]
</script>

<header class={'sticky z-[15] top-0 duration-200 px-6 flex items-center justify-between ' + 
    (y > 0 ? 'py-5 bg-stone-900/95 shadow-md border-b border-stone-800 backdrop-blur-sm' : 'py-5 shadow-md border-b border-yellow-800 backdrop-blur-md')}>
    <h1 class="text-xl font-bold">
        Sustainability
    </h1>
    <nav class="sm:flex items-center gap-8 hidden">
        {#each tabs as tab, index}
        <a href={tab.link} class="duration-200 hover:text-yellow-400 text-lg">
            <span>{tab.name}</span>
        </a>
        {/each}
    </nav>
</header>