<script>
    import { writable, get } from 'svelte/store';
    import { onMount, onDestroy } from 'svelte';
  
    // Create a writable store
    const userInput = writable('');
  
    onMount(() => {
      // Only runs in the browser
      // Expose userInput to window
      window.userInput = '';
  
      // Set up a manual subscription to handle reactivity
      const unsubscribe = userInput.subscribe(value => {
        window.userInput = value;
      });
  
      // Polling for manual changes to window.userInput
      const interval = setInterval(() => {
        const currentUserInput = get(userInput);
        if (window.userInput !== currentUserInput) {
          userInput.set(window.userInput);
        }
      }, 300); // Check every 300ms
  
      // Cleanup on component destruction
      onDestroy(() => {
        clearInterval(interval);
        unsubscribe();
      });
    });
  
    // Manual logging (Svelte 5 doesn't have $: syntax for store values)
    let userInputValue = '';
    const unsubscribeLog = userInput.subscribe(value => {
      userInputValue = value;
      console.log(value);
    });
  
    // Cleanup log subscription
    onDestroy(() => {
      unsubscribeLog();
    });
  </script>
  
  <!-- Input bound directly to the store -->
  <input type="text" placeholder="Type something" bind:value={$userInput} />
     