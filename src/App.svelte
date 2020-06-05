<script>
	export let name = 'Ethan';
	import Comp from "./components/comp.svelte";
	import Clock from "./components/clock.svelte";

	function handleClick() {
		alert('clicked');
	}

</script>

<main>
	<h1>Hello {name}!</h1>
	<Comp/>
	<Clock/>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		background : aqua;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
	p {
		color: chocolate;
		font-size: 2em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>