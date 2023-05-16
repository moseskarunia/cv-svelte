<script lang="ts">
	import Strawberry from '$lib/assets/strawberry.jpeg';
</script>

<h1>Welcome to SecondRoute</h1>

<!--Image from link-->
<img
	src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Garden_strawberry_%28Fragaria_%C3%97_ananassa%29_single2.jpg/800px-Garden_strawberry_%28Fragaria_%C3%97_ananassa%29_single2.jpg"
	alt="Strawberry"
/>

<!--Image from assets-->
<img src={Strawberry} alt="Strawberry" />

<a href="/">Go to main page</a>

<style>
	img {
		display: none;
	}
</style>
