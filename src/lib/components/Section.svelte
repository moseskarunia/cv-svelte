<script lang="ts">
	import Icon from 'svelte-awesome';
	import type { IconType } from 'svelte-awesome/components/Icon.svelte';

	export let iconData: IconType;
	export let title: string;
</script>

<div class="container">
	<div class="section-title">
		<Icon data={iconData} />
		{title}
	</div>
	<slot />
</div>

<style>
	.section-title {
		display: flex;
		align-items: center;
		gap: 16px;
		background-color: #ffeb3b;
		border-left: 4px solid #fbc02d;
		color: black;
		padding: 8px 16px;
		text-transform: UPPERCASE;
		font-weight: 500;
	}
	.container {
		display: flex;
		flex-direction: column;
		gap: 16px;
	}
</style>
