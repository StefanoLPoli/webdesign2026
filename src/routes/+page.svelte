<script>
    console.log('Logsss!');
    let count = $state(0);
    let doubled = $derived(count * 2);
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>

<button onclick={()=> count++}>
    Click: {count}
</button>

<span>Doubled: {doubled}</span>

<style>
	h1 {
		color: deepskyblue;
	}
</style>