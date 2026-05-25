<script lang="ts">
	import Componente1 from './Componente1.svelte';
	import Componente2 from './Componente2.svelte';
	import { contador } from './minhaStoreLocal.svelte';

	let meuEstado = $state(1);
</script>

<div>INÍCIO DO +PAGE.SVELTE</div>
<Componente1 bind:propEstado={meuEstado} />
<Componente2 propEstado={meuEstado} />
<div>FINAL DO +PAGE.SVELTE</div>
VALOR DO ESTADO: {meuEstado}

<button style="background-color: #007bff; color: white; border: none; " onclick={() => meuEstado++}
	>+</button
>

<div class="bg-red-400">
	<div>A PARTIR DE AGORA É MINHA EXPLICAÇÃO SOBRE STORE:</div>
	{contador.valor}
	<button
		style="background-color: #007bff; color: white; border: none; "
		onclick={() => contador.valor++}
	>
		+
	</button>
</div>
