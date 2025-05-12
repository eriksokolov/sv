<script>
function lastletter(str) {
    return str.charAt(str.length -1);
}

let list = ['foo', 'bar', 'baz'];
let i = 0;
let rIndex;

while (i < 1) {
    rIndex= Math.floor(Math.random()* list.length);
    i = i + 1;
}


let foo = list[rIndex];
let funky = lastletter(foo);
console.log(foo)
console.log(funky)


</script>

<style>
    h1 {
        color: purple;
    }
</style>

<h1>Hello name!</h1>