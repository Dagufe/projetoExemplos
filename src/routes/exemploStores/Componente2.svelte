<script lang="ts">
	import { contador } from './minhaStoreLocal.svelte';

	let {
		propEstado,
	}: {
		propEstado: number;
	} = $props();
</script>

<div>
	EU SOU O COMPONENTE 2 E AQUI DENTRO O ESTADO É: {propEstado}
	<button
		style="background-color: #007bff; color: white; border: none; "
		onclick={() => propEstado++}>+</button
	>
</div>

<div class="bg-yellow-400">
	<div>A PARTIR DE AGORA É MINHA EXPLICAÇÃO SOBRE STORE:</div>
	{contador.valor}
	<button
		style="background-color: #007bff; color: white; border: none; "
		onclick={() => contador.valor++}
	>
		+
	</button>
</div>
