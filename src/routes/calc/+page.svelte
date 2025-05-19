<script>
    let numpad = [1,2,3,4,5,6,7,8,9];
    let select = "";
    let plus = "+"; 
    let minus = "-";
    let equals = "=";
    let result = ""
    let reset = "esc";

    function calculate() {
            result = eval(select);
    }
</script>
<style></style>

<div>
    {#each numpad as key}
        <button on:click={() => select += key}> {key}</button>    
    {/each}
</div>
<div>
    <button on:click={() => select = select + plus}> 
        {plus}        
    </button>
    <button on:click={() => select = select + minus}>
        {minus}
    </button>
</div>
<div>
    <button on:click={calculate()}>
        {equals}
    </button>
</div>
<div>
    <button on:click={()=> select = ""}>{reset}</button>
</div>
<p>{select}</p>
<p>{result}</p>
