<script lang="ts">
	import type { Snippet } from 'svelte';

	let { children }: { children: Snippet } = $props();
</script>

<div>INÍCIO DO LAYOUT</div>
{@render children()}
<div>FIM DO LAYOUT</div>
