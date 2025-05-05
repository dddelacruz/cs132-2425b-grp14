<script>
	import AboutCard from '$lib/aboutcard/AboutCard.svelte';
	import avatar from '$lib/assets/avatar.png'
	import avatar_delacruz from '$lib/assets/avatar_delacruz.png'
	import avatar_fadri from '$lib/assets/avatar_fadri.png'

	let about = {
		"avatar" : avatar,
		"name" : "name1",
		"desc" : "desc2",
		"link" : "link3",
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


<AboutCard {...delacruz}/>
<AboutCard {...fadri}/>
<AboutCard {...about}/>


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
	}

	.column {
		flex: 33.33%;
		padding: 5px;
	}

	
</style>
