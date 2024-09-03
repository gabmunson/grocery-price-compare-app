<script lang="ts">
	let isFocused: boolean = true;

	let searchQuery = '';

	function searchWebsites() {
		console.log( searchQuery );
	}
</script>

<main-container>
	<div>
		<h2 class="h2">Search for a grocery item:</h2>
	</div>
	<div class="search-bar">
		<div class="input-group input-group-divider grid-cols-[auto_1fr_auto]">
			<input type="search" placeholder="Search..." bind:value={searchQuery}/>
			<button class="variant-soft-primary" on:click={searchWebsites}><h6 class="h6">Search</h6></button>
		</div>
	</div>
</main-container>

<style>
	main-container {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100%;
		width: 100%;
	}

	.search-bar {
		padding: 50px;
	}
</style>

