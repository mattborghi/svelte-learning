<script lang="ts">
	// export let name: string;
	let name2: string;

	function setName(name: Event): void {
		console.log(name)
		// console.log("given name2: " + name2, "set name2 to: " + namen);
		// name2 = namen;
	}
</script>

<main>
	<label for="name">Name:</label><input id="name" type="text" value={setName}>
	<h1>Hello {name2}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>