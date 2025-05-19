<script>
    let toggles = [];
    let links = ["https://www.youtube.com/@ClearCode", "https://en.wikipedia.org/wiki/Oslo_Stock_Exchange", "https://copy.sh/v86/?profile=archlinux"]
    let color = "#69923e";

    const foo = () => {
        toggles = toggles.length ? [] : ["youtube","wikipedia","arch",4,5]
    };
</script>
<style>
    :global(body){
        margin:0px;
        background-color:lightgrey;
        display: flex;
    }
    .button{
        color: white;
    }
</style>

<div>
    <div class="button" on:click={foo}>
        <svg fill={color} height="25px" width="25px">
            <rect height= "100px" width="100px"/>
        </svg>
    </div>
    {#each toggles as toggle, i}
        <a href={links[i]} target="_blank">{toggle}</a>
        <br>
    {/each}
</div>