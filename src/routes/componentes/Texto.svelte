
<script>
	export let inicio=0;
  
  let count = inicio;
  
	$: termino=`ya acabé ${count*5} veces`;

	function handleClick() {
		count += 1;
    if (count >= 10) {
		alert('count is dangerously high!');
		count = 0;
	}
	}
</script>

<button on:click={handleClick}>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>

<p>Este es el primer texto de la página web</p>
<p>{termino}</p>



<style>
  p {
    background-color: blue ;
    font-size: medium;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    color: white;
  }
</style>

