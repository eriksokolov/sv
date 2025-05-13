<script>
	let four = 4;
    let pic = "favicon.png";
    let none = "none"
    
    function change() {
        pic = "malevich.jpg"
        none = "hey"
    }
    
</script>

<style>
:global(body) {
	height: 100%;
	margin: 0;
	display: flex;
	justify-content: center;
	align-items: center;
}

.board {
	background-color: black;
	width: 400px;
	height: 400px;
	display: grid;
	grid-template-columns: repeat(2, 1fr);
	grid-template-rows: repeat(2, 1fr);
	gap: 2px;
}

.field {
	border: 1px solid white;
	display: flex;
	justify-content: center;
	align-items: center;
}

.field img {
	width: 80%;
	height: auto;
}
</style>

<div class="board">
	{#each Array(four) as _, i}
		<div class="field">
			<img src="/{pic}" alt="placeholder" on:click={change()} style="display:{none};"/>
		</div>
	{/each}
</div>
