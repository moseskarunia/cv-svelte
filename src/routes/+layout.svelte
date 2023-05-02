<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
  <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;500&family=Peralta&display=swap"
    rel="stylesheet">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <script src="https://kit.fontawesome.com/d0c488930b.js" crossorigin="anonymous"></script>
</svelte:head>

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
