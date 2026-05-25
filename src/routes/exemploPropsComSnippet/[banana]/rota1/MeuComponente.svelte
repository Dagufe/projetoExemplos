<script lang="ts">
	import type { Snippet } from 'svelte';

	let {
		valor,
		children,
	}: {
		valor: string;
		children: Snippet;
	} = $props();
</script>

ESTOU DENTRO DO COMPONENTE
{valor}
{@render children()}
