<script>
	let count = 0;
	//antes de declarar nuestra variable computada debemos de declarar $: despues la variable para hacer que trabaje con normalidad
	$: double = count * 2;
	function handleClick() {
		count += 1;
	}
	$: {
		console.log(count)
	}
	$: if(count > 5) {
		alert('5');
	}
</script>

<main>
	<button on:click="{ handleClick }">
		Clicked
		{ count }
	</button>
	<p>{ double }</p>
</main>

