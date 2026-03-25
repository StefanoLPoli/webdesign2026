<script>
    let props = $props();
    let count = $state(props.initialCount);
    let doubled = $derived(count * 2);
</script>

<h3>Clicks counter!</h3>

<button onclick={()=> count++}>
    Click: {count}
</button>

<span>Doubled: {doubled}</span>