<script>
	let message = 'Bienvenido al curso de svelte'
	let num = 5
	let description = 'logo de pokemon'
	let src = 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/98/International_Pok%C3%A9mon_logo.svg/1200px-International_Pok%C3%A9mon_logo.svg.png'
</script>

<main>
	<h1>{ message.toUpperCase() }</h1>
	<p>{ num + 5 }</p>
	<img { src } alt={ description } />
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