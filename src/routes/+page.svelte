<script>
	let frutas = ['Maçã', 'Banana', 'Laranja'];
</script>

<ul>
	{#each frutas as fruta (fruta)}
		<li>{fruta}</li>
	{/each}
</ul>
