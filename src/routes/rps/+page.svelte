<script>
    let playerChoice = "";
    let result = "";
    const options = ["rock", "paper", "scissors"];

    function getComputerChoice() {
        const computer = Math.floor(Math.random() * options.length);
        return options[computer];
    }

    function play(choice) {
        playerChoice = choice;
        const pc = getComputerChoice();

        if (choice === pc) {
            result = "Tie!";
        } else if (
            (choice === "paper" && pc === "rock") ||
            (choice === "rock" && pc === "scissors") ||
            (choice === "scissors" && pc === "paper")
        ) {
            result = `You win! PC chose ${pc}`;
        } else {
            result = `You lose! PC chose ${pc}`;
        }
    }


    const name = "name";
    const age = "age";
    console.log(`Hello foo bar lorem ${name} baz buzz ${age} ciz cuz`)
    console.log(age.length);
</script>

<div>
    <h1>Rock Paper Scissors</h1>
    {#each options as option}
        <button on:click={() => play(option)}>{option}</button>
    {/each}
    {#if result}
        <p>{result}</p>
    {/if}
</div>
