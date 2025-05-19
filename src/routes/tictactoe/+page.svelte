<script>
    let grids = [1,2,3,4,5,6,7,8,9];
</script>

<style>
    :global(body){
        display: flex;
        text-align: center;

    }
    .grid{
        display: grid;
        grid-template-columns: repeat(3,1fr);
        margin: 0;
        padding: 0;
        gap: 0;
    }
    .grid > div{
        width: 100px;
        height: 100px;
        padding: 0px;
        margin: 0;
        box-sizing: border-box;
    }
    .grid > div:hover rect {
        fill: orange;
    }

    .grid svg{
        display: block;
    }
</style>

<div class = "grid">
    {#each grids as grid}
        <div> 
            <svg width="100px" height="100px" >
                <rect width="100px" height="100px" stroke="orange" stroke-width="1">
                </rect>
            </svg>
        </div>
    {/each}
</div>
