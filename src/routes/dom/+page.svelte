<script>
    import {onMount, onDestroy} from 'svelte';

    const funion = () => {
        console.log('foo');
        let head = document.querySelector('head');
        let newTitle = document.createElement('title');
        newTitle.textContent = "foo";
        head.appendChild(newTitle);
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

