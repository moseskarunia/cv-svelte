<div class="parent">
	<div class="sidebar" />
	<div class="content">
		<slot />
	</div>
</div>

<style>
	:global(*) {
		margin: 0;
		padding: 0;
	}
	:global(html, body) {
		width: 100%;
		height: 100%;
	}
	.parent {
		width: 100%;
		height: 100%;
		display: flex;
		flex-direction: row;
	}
	.sidebar {
		background-color: blue;
		width: 200px;
		height: 100%;
	}
	.content {
		display: flex;
		flex-direction: column;
	}
</style>
