<style>
    :global(body){
        height: 100vh;
        display:grid;
        justify-content:center;
        align-content: center;
        background-color: black;
    }
    .canvas{
        height: 30rem;
        width: 30rem;
        background: #f4f4f4;
    }

</style>
<div class="canvas">
  <svg viewBox="0 0 1 1">
    <polygon points="0.5,0.9 0.5,0.7 0.7,0.7 0.7,0.9" fill="orange"></polygon>
    <polygon points="0.6,0.6 0.6,0.5 0.8,0.5 0.8,0.6" fill="black" transform="rotate(-22 0.8 0.5)"></polygon>
    <polygon points="0.4,0.5 0.4,0.4 0.7,0.4 0.7,0.5" fill="red" transform="rotate(-22 0.8 0.5)"></polygon>
    <polygon points="0.5,0.475 0.5,0.4 0.6,0.4 0.6,0.47" fill="black" transform="rotate(-22 0.6 0.7)"></polygon>
    <polygon points="0.4,0.3 0.4,0.28 0.7,0.28 0.7,0.3" fill="blue" transform="rotate(-30 0.7 0.5)"></polygon>
    <polygon points="0.54,0.26 0.53,0.18 0.67,0.17 0.67,0.26" fill="orange" transform="rotate(-30 0.7 0.5)"></polygon>
  </svg>
</div>
