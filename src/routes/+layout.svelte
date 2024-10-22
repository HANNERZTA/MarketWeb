<script>
	import Header from './Header.svelte';
	import '../app.css';
</script>


<body>
	<div class="app">
		<main>
			<Header/>
			<slot />
		</main>
	</div>
</body>
<style>
	body
	{
		background: white;
		background-attachment: fixed;
	}
</style>