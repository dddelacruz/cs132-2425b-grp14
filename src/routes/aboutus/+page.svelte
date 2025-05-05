<script>
	import AboutCard from '$lib/aboutcard/AboutCard.svelte';
	import avatar from '$lib/assets/avatar.png'
	import avatar_delacruz from '$lib/assets/avatar_delacruz.png'
	import avatar_fadri from '$lib/assets/avatar_fadri.png'
	import avatar_macaraig from '$lib/assets/avatar_macaraig.jpg'

	let about = {
		"avatar" : avatar_macaraig,
		"name" : "Manuel Carlo D. Macaraig",
		"desc" : "Currently a graduating 4th year BS Computer Science student. If he's not coding, he's either making beats or cool posters : ]",
		"link" : "https://github.com/mdmacaraig",
	}
	let fadri = {
		"avatar" : avatar_fadri,
		"name" : "Vincent Paul C. Fadri",
		"desc" : "4th year BS Computer Science Student:)",
		"link" : "https://github.com/vpcfadri1",
	}

	let delacruz = {
		"avatar" : avatar_delacruz,
		"name" : "Diana Mae D. de la Cruz",
		"desc" : "Currently a graduating 4th year BS Computer Science student under the Scientific Computing Laboratory.\nUsually found playing maimai.",
		"link" : "https://github.com/dddelacruz",
	}
</script>

<svelte:head>
	<title>Home</title>
	<meta name="About us" content="About us" />
</svelte:head>

<section>
	<h1>About the team</h1>
</section>

<div class="row">
	<div class="column">
		<AboutCard {...delacruz}/>
	</div>
	
	<div class="column">
		<AboutCard {...fadri}/>
	</div>

	<div class="column">
		<AboutCard {...about}/>
	</div>
</div>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
		border: 2px solid gray;
  		border-radius: 5px;
		width: auto;
		padding: 20px;
		background-color: rgba(255, 255, 255, 0.8);
		margin: 20px auto;
	}

	h1 {
		width: 100%;
		margin: auto;
	}
	.row {
		display: flex;
		flex-direction: row;
    	flex-wrap: wrap;
	}

	.column {
		flex: 30%;
		padding: 5px;
	}

	
</style>
