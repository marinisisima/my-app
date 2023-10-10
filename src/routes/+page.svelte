<script>
	import Texto from "./componentes/Texto.svelte";
  import { Styles } from 'sveltestrap';

  let nombre="México"
  let nombre2="Pozolero"
  let src = '/gift2.gif';
	let alt = 'POCOYO baila';
  let inicio=3;
</script>


<h1>Carpe Diem</h1>
<h1>Viva ¡{nombre.toUpperCase()}! Jijos del maíz... ({nombre2})</h1>
<h1>Marinisisima 140923</h1>
<img {src} {alt} baila. />
<Texto {inicio}/>
<Styles />






