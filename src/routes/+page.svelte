<script lang="ts">
    let count = $state(0)
</script>

<div class="flex-gap">
    <input type="text" bind:value={count}>
    <button onclick={() => count = count + 1}>Count</button>
</div>

<a href="./temperature/">temperature converter</a>