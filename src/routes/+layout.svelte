<script>
	import Nav from '$lib/components/folder/Nav.svelte';
	import { store } from '$lib/store';
	import 'bootstrap/dist/css/bootstrap.min.css';
	import 'bootstrap/dist/js/bootstrap.min.js';
	console.log($store);
</script>

<div class="container pt-5">
	<div class="d-flex">
		<Nav folders={$store.Folders} />
		<slot />
	</div>
</div>
