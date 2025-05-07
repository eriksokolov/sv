<script lang="ts">
    let c = $state(0)
    let f = $state(0)
</script>

<div>
    <input type="number" bind:value={c} /> Celsius =
    <input type="number" bind:value={f} /> Fahrenheit
</div>


<style>
    input[type="number"] {
        max-width: 10ch;
    }
</style>