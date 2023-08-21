<script lang="ts">
	import Day from './lib/Day.svelte';
</script>

<main>
	<div class="header"><h1>MYFC</h1></div>
	<div class="body">
		<Day date={new Date('2023-08-21')} am={['🏃', '🚶']} pm={['🚶', '🏃']} kg={92} />
	</div>
</main>

<style>
	h1 {
		font-size: 1.25em;
		margin: 0;
		padding: 1em 0.5em;
	}

	.header {
		background-color: cadetblue;
	}

	.body {
		padding: 0 0.5em;
		border-radius: 3px;
		width: calc(100% / 7);
	}
</style>
