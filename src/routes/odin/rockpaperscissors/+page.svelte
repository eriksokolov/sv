<script>

    function getComputerChoice(){
        /*random number, 0,1,2*/
        let pc = Math.floor(Math.random() * 3);
        console.log(pc);
        return(pc);
    }
    let result = getComputerChoice();
    console.log(result);


</script>