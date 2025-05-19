<script>
</script>
<style>
    :global(body){
        margin: 0px;
    }

    .box {
        display: grid;
        grid-template-columns: repeat(2,1fr);
        justify-items: center;
        background-color: #000;
        color: #fff;
    }
    .svg{
        width: 400px;
        height: 300px;
        border: 1px solid #000;
        margin-bottom: 50px;
    }
</style>

<div class="box">
        <svg class="svg">
            <rect width="200" height="150" fill="#69923e" x="200px" y="150px" rx="2" />
            <circle cx="50%" fill="#69923e" cy="50%" r="75" />
        </svg>
    <svg class="svg">
    </svg>
    <svg class="svg"></svg>
</div>