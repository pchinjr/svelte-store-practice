<script>
  import Counter from './components/Counter.svelte'
  import Clock from './components/Clock.svelte'
  export let name
</script>

<main>
	<h1>{name}</h1>
  <Counter/>
  <Clock/>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>