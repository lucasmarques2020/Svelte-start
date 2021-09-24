<script>
	let contador = 0;
	const aumentar = ()=>{
		contador++;
	}
	const apagar = ()=>{
		contador=0;
	}
</script>

<main>
	<h1>Brincando com svelte</h1>
	<h2>Resultado contador: {contador}</h2>
	<button on:click={aumentar}>AUMENTAR</button>
	<button on:click={apagar}>APAGAR</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>