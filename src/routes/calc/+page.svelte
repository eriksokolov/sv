<script>
    let numpad = [1,2,3,4,5,6,7,8,9];
    let select = "";
    let plus = "+"; 
    let minus = "-";
    let times = "*";
    let divide = "/";
    let equals = "=";
    let result = ""
    let reset = "esc";

    function calculate() {
            result = eval(select);
    }
</script>
<style>
    :global(body){
        background-color:#2c2b29;
        color: white;
    }
    .plastic{
        background-color:#4b4847;
        display: flex;
        align-items: center;
        
    }
    .key{
        background-color:#69923e;
    }
    .math{
        all: unset;
        background-color:transparent;
        color: white;
        display: flex;
        align-items: center;
        width: 25px;
        height: 25px;
        justify-content: center;
        border: 1px solid white;
    }
    .rest{
        all: unset;
        background-color:transparent;
        color: white;
        display: flex;
        align-items: center;
        width: 25px;
        height: 25px;
        justify-content: center;
        border: 1px solid white;
    }
</style>

<div class="plastic">
    <div class="numpad">
        {#each numpad as key}
            <button class="key" on:click={() => select += key}> {key}</button>    
        {/each}
    </div>
    <div>
        <button class="math" on:click={() => select = select + plus}> 
            {plus}        
        </button>
        <button class="math" on:click={() => select = select + minus}>
            {minus}
        </button>
        <button class="math" on:click={() => select = select + times}>
        {times}
        </button>
        <button class="math" on:click={() => select = select + divide}>
            {divide}
        </button>
    </div>
    <div>
        <button class="rest" on:click={calculate()}>
            {equals}
        </button>
    </div>
    <div>
        <button class="rest" on:click={()=> select = ""}>{reset}</button>
    </div>
    <p>{select}</p>
    <p>{result}</p>
</div>