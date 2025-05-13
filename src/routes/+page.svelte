<script>
let euppertext= "Hello, I am Erik, I am German, I love studying russian, love to read and want to become a front end developer."
let etitle= "Site"

function invertion() {
    console.log("invert")
    document.body.style.filter = "invert(1)";
    document.body.style.backgroundColor = "black";
    document.getElementById("malevich").style.filter = "invert(1)";
    etitle = "Сайт"
    euppertext = "приветь, я Эрик, я немец, люблю выучить русский, люблю читать, и хочу стать программистам."
}

function funion() {
    document.body.style.filter = "invert(0)";
    document.body.style.backgroundColor = "white";
    etitle = "Site"
    euppertext = "Hello, I am Erik, I am German, I love studying russian, love to read and want to become a front end developer."
}
</script>

<div id="title">{etitle}</div>

<br>
<hr>
<br>

<div id="uptext">
    {euppertext}
</div>

<br>
<hr>
<br>

<div id="malevichCon" >
    <img id="malevich" src=/malevich.jpg alt="malevich's square" on:mouseover={invertion}>
</div>

<br>
<hr>
<br>

<div id="buttonCon">
    <button id="button" on:click={funion}>Back to english</button>
</div>

<style>

    #title{
        font-size: 30px;
        text-align: center;
    }
    #uptext{
        font-size: 20px;
        text-align: center;
    }
    #malevichCon{
        text-align: center;
    }
    #malevich{
        height: 100px;
        width: 100px;
    }
    #buttonCon{
        text-align: center;
    }
    


</style>

