<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children }: { children: Snippet } = $props();
</script>

<div>INÍCIO DO LAYOUT INTERNO</div>
{@render children()}
<div>FIM DO LAYOUT INTERNO</div>
