<script>
	import { onMount } from 'svelte'

	onMount(async () => {
		const wasm = await import('../pkg')
		wasm.greet('world')
	})

	export let name;
</script>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Hello {name}!</h1>