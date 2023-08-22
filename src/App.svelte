<script lang="ts">
	import Day from './lib/Day.svelte';
</script>

<main>
	<div class="header"><h1>MYFC</h1></div>
	<div class="body">
		<Day date={new Date('2023-08-21')} am={['🏃', '🚶']} pm={['🚶', '🏃']} kg={92} />
		<Day date={new Date('2023-08-22')} am={['🏃', '🚶']} pm={['🚶']} kg={undefined} />
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
</style>
