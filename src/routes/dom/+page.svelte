<script>
    import {onMount, onDestroy} from 'svelte';

    const funion = (e) => {
        console.log('foo');
        let body = document.querySelector('body');
        let newTitle = document.createElement('div');
        newTitle.textContent = "foo";
        body.appendChild(newTitle);
        console.log(e.target);
        newTitle.innerHTML = e.type; 
    }

    onMount(() => {
        const btn = document.getElementById('btn');
        btn.addEventListener('click', funion);
    
        onDestroy(() => {
            btn.removeEventListener('click', funion);
        });
    });
</script>
<style>
    :global(body){
        background-color: black;
        color: #fff;
        font-family: sans-serif;
    }
</style>

<div id="btn">X</div>

