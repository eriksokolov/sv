<script>
    let toggles = [];
    let color = "blue";

    const foo = () => {
        toggles = toggles.length ? [] : [1,2,3,4,5]
    };
</script>
<style>
    :global(body){
        margin:0px;
    }
</style>

<div>
    <div class="button" on:click={foo}>
        <svg fill={color} height="25px" width="25px">
            <rect height= "100px" width="100px"/>
        </svg>
    </div>
    {#each toggles as toggle}
        <p>{toggle}</p>
    {/each}
</div>