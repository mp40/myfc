<script lang="ts">
	export let time: 'am' | 'pm';
	export let activites: string[];
</script>

<div>
	<span>{time}</span>
	{#each activites as a}
		<span>{a}</span>
	{/each}
</div>
