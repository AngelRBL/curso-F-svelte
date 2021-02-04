<script>
	let numbers = [1, 2, 3, 4];

	function addNumber() {
		numbers.push(numbers.length + 1);
		numbers = [ ...numbers, numbers.length ];
	}

	$: sum = numbers.reduce((t, n) => t + n , 0);
</script>
<p>{ numbers.join(' + ') } = { sum }</p>
<button onclick={ addNumber }>add number</button>
<main>

</main>

