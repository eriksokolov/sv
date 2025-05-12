<script>
	let gridSize = 16;

	// handle hover event on each cell
	function handleHover(event, i) {
		console.log(`Hovered over square ${i + 1}`);
		event.target.style.backgroundColor = 'orange';
	}

	// handle mouse out event to reset the cell color
	function handleMouseOut(event) {
		event.target.style.backgroundColor = 'lightgray';
	}

	// double the grid size
	function double() {
		gridSize = gridSize * 2;
	}
</script>

<style>
	.grid {
		display: grid;
		aspect-ratio: 1 / 1;
		width: 512px;
		border: 2px solid #000;
	}

	.cell {
		background-color: lightgray;
		border: 1px solid #000;
		display: flex;
		align-items: center;
		justify-content: center;
		cursor: pointer;
		font-size: 10px;
	}
</style>

<!-- Button to double the grid size -->
<button on:click={double}>squares * 2</button>

<!-- Grid container with dynamic number of columns and rows -->
<div
	class="grid"
	style={`grid-template-columns: repeat(${gridSize}, 1fr); grid-template-rows: repeat(${gridSize}, 1fr);`}>
	{#each Array(gridSize * gridSize) as _, i}
		<div
			class="cell"
			role="button"
			aria-label={`Square ${i + 1}`}
			on:mouseover={(event) => handleHover(event, i)}
			on:mouseout={handleMouseOut}>
		</div>
	{/each}
</div>
