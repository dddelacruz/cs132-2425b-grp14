<script lang="js">
	import '../app.css';
    import Footer from '../components/Footer.svelte';
    import Header from '../components/Header.svelte';
	let { children } = $props();
	let y;
	let innerHeight = 0;
	let innerWidth = 0;

	function goTop(){
		document.body.scrollIntoView()
	}
</script>



<div class="relative flex flex-col max-w-[1400px] mx-auto w-full text-sm sm:text-base min-h-screen">
	<div class={'fixed bottom-0 w-full duration-200 flex p-10 z-[10] ' + (y > 0 ? 'opacity-100 pointer-events-auto' : 'pointer-events-none opacity-0')}>
		<!-- svelte-ignore a11y-click-events-have-key-events -->
		<button on:click={goTop} class="ml-auto rounded-full bg-stone-900 text-yellow-400 px-3 sm:px-4 hover:bg-stone-800 cursor-pointer">
			<i class="fa-solid fa-arrow-up grid place-items-center aspect-square"/>
		</button>
	</div>
	<Header {y}/>
	{@render children()}
	<Footer/>
</div>


<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth></svelte:window>
