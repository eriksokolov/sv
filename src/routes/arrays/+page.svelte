<script>
    let books = ["foo", "bar", "baz", "far", "faz"];
    let inputValue = "";

    const rmv = () => {
        books = books.slice(0, -1);
    }

    const add = () => {
        books = [...books, inputValue]; 
        inputValue = "";
    }
</script>

<div>
    {#each books as book}
        <p on:click={rmv}>{book}</p>
    {/each}
</div>

<div>
    <input 
        bind:value={inputValue}
        on:keydown={(event) => {if(event.key === "Enter") add();}}
    >
</div>