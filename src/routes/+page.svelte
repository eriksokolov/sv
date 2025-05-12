<script>

function invertion() {
    console.log("invert")
    document.body.style.filter = "invert(1)";
    document.body.style.backgroundColor = "black";
    document.getElementById("malevich").style.filter = "invert(1)";
}

</script>

<div id="title">Website</div>

<br>
<hr>
<br>

<div id="uptext">
    приветь, я Эрик, я немец, люблю выучить русский, люблю читать, и хочу стать программистам.
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


</style>

