<script lang="ts">
	import Activities from './Activities.svelte';

	export let date: Date;
	export let am: string[];
	export let pm: string[];
	export let kg: number | undefined;
</script>

<div class="card">
	<span>{`${date.getDate()} ${date.toLocaleString('default', { month: 'short' })}`}</span>
	<Activities time={'am'} activites={am} />
	<Activities time={'pm'} activites={pm} />
	{#if kg}
		<span>{`${kg}kg`}</span>
	{/if}
</div>

<style>
	.card {
		margin-top: 1em;
		padding: 0.5em;
		background-color: white;
		box-shadow: 0px 1px 5px 3px rgba(171, 153, 153, 0.75);
		-webkit-box-shadow: 0px 1px 5px 3px rgba(171, 153, 153, 0.75);
		-moz-box-shadow: 0px 1px 5px 3px rgba(171, 153, 153, 0.75);
	}
</style>
