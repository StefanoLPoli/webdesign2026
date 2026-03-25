<script>
    let {initialCount: count = $bindable()} = $props();
    let doubled = $derived(count * 2);
</script>

<h3>Clicks counter!</h3>

<button onclick={()=> count++}>
    Click: {count}
</button>

<span>Doubled: {doubled}</span>