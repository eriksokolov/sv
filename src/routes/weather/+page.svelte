<script>
  let imageUrl = '';

  // Загружаем гифку при монтировании компонента
  onMount(async () => {
    const res = await fetch('https://api.giphy.com/v1/gifs/translate?api_key=miVNpodeyiDJ9JrB9mRbd2OJZbtriYF1&s=cats', { mode: 'cors' });
    const data = await res.json();
    imageUrl = data.data.images.original.url;
  });

  import { onMount } from 'svelte';
</script>
<style>
    :global(body){
        background-color: black;
        display: flex;
        justify-content: center;
        padding: 2rem;
    }
</style>

<h1>Hello</h1>
{#if imageUrl}
  <img src="{imageUrl}" alt="Cat gif">
{:else}
  <p>Loading...</p>
{/if}
