<script>
	let contador = 0;
	const aumentar = () =>{
		contador++;
	}
	const limpar = () =>{
		contador=0;
	}
	const diminuir = () =>{
		contador--;
	}
</script>

<main>
	<h1>Brincando com svelte</h1>
	<h2>Aumentando o número com botão</h2>
	<h2>{contador}</h2>
	<button on:click={aumentar}>AUMENTAR</button>
	<button on:click={limpar}>LIMPAR</button>
	<button on:click={diminuir}>DIMINUIR</button>
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