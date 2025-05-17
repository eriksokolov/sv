<script>
    let tiles = [1,2,3,4,5,6,7,8,9];
    let selected = [];
    let result = 0;
    let tools = [
        (a,b) => a+b,
        (a,b) => a-b,
        (a,b) => a*b,
        (a,b) => a/b
    ]
    let toolsign = [
        "+",
        "-",
        "*",
        "/",
    ]


</script>
<style>
.key {
    background-color:blueviolet;
    border: 1px solid white;
}
.reset{
    background-color:forestgreen;
}
.tools{
    background-color:orange;
}
</style>

{#each tiles as key}
    <div class="key" on:click={() => selected = [...selected, key]}>
        {key}
    </div>
{/each}
<hr>
<p>1. {selected.join()}</p>
<p>2. {result}</p>
<b class="reset" on:click={() => {
    selected = [];
    result = 0;
}}>esc</b>
{#each tools as tool, i}
<div>
    <b class="tools"
        on:click={tools[i]} 
    >{toolsign[i]}</b>
</div>
{/each}