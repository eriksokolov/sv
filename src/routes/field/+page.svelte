<script>
let arr = ['1', '2', '3', '4', '5', '6', '7', '8', '9'];
let border = "2px solid white"
let hoveredIndex = null;
let selectedIndex = null;

const changecss= (event, i) => {
    event.target.style.border  = "2px solid  orange";
    hoveredIndex = i;
};
const revertcss= event => {
    event.target.style.border = border; 
    hoveredIndex = null;
}
const toggleSelect = (i) => {
    selectedIndex = selectedIndex === i ? null :i;
};
</script>
<style>
:global(body){
    margin:0;
    display: flex;
    justify-content: center;
    
    
}
.board{
    background-color: green;
    height: 400px;
    width: 400px;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3,1fr);
}
.key{
    background-color:black;
    color: white;
    display: flex;
    justify-content: center;
    border:2px solid white;
    align-items: center;

}
</style>

<div class = "board">
    {#each arr as item, i} 
        <div 
            class = "key" 
            on:mouseenter={(e) => changecss(e, i)}
            on:mouseleave={revertcss}
            on:click={() => toggleSelect(i)}
        >
            {#if hoveredIndex === i || selectedIndex === i}
                <img src="/favicon.png" alt="icon" />
            {:else}
                {item}
            {/if}
        </div>
    {/each}
</div>