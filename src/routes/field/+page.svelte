<script>
let arr = ['1', '2', '3', '4', '5', '6', '7', '8', '9'];
let border = "2px solid white"

const changecss= event => event.target.style.border  = "2px solid  orange";
const revertcss= event => event.target.style.border = border; 

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
        <div class = "key" 
            on:mouseenter={changecss}
            on:mouseleave={revertcss}
        >
            {item}
        </div>
    {/each}
</div>