<script>
	export let folders;
	$: console.log(folders);
</script>

<nav class="nav flex-column">
	{#each folders as folder}
		<a class="nav-link" aria-current="page" href="folder/{folder.id}">{folder.name}</a>
	{/each}
</nav>
