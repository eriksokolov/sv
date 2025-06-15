<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    :global(body){
        height: 110vh;
        margin: 0;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows:0.1fr 0.8fr auto;
        grid-template-areas:
        "header header"
        "content orange"
        "footer footer";
        background-color: #eae6db;
        font-family: Arial;
    }

    .headerContainer{
        grid-area: header;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-areas: "left right";
        background-color: #000; 
        color: #eae6db;
    }
    .left-header{
        grid-area: left;
        padding-left: 1rem;
        display:flex;
        justify-content: start;
        align-items: center;
    }
    .right-header{
        grid-area: right;
        padding-right: 1rem;
        display: flex;
        justify-content: end;
        align-items: center;

    }
    .left-header p{
        padding-left: 1rem;
    }
    .right-header p{
        padding-right: 1rem;
    }
    .right-header a{
        all: unset;
        padding-right: 1rem;
    }
    
    .logo{
        height: 2rem;
        width: 2rem;
        background-color: #fff;
    }
    .contentContainer{
        height: 100%;
        width: 100%;
        grid-area: content;
        padding: 1rem;
        margin-top: 1rem;
        padding-bottom: 6rem;
        display:grid;
        align-content: space-between;
        transform: rotate(-10deg);
    }
    
    .orangeContainer{
        padding: 1rem;
        grid-area: orange;
        display: grid;
        align-items: end;
        justify-content: start;
    }
    .first-content{
        height: 4rem;
        width: 6rem;
        background-color: #da9b01;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-left: 20rem;
    }
    .blue-content{
        height: 2.5rem;
        margin-left: 5rem;
        background-color: #150937;
        color: #eae6db;
        display:flex;
        align-items: center;
        justify-content: center;
        font-size: 1.5rem;
        font-family: "sans-serif";
    }
    .latter-content{
        display:grid;
        margin: 0;
        transform: rotate(5deg)
    }
    .black-content {
        background-color: black;
        color: #eae6db;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    #upper-black{
        height: 3rem;
        width: 4rem;
        margin-left: 15rem;
        transform: rotate(2deg);
    }
    .red-content {
        height: 6rem;
        width: 22rem;
        background-color:#e01e00;
        color: #eae6db;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-left: 12rem;
        font-size: 4rem;
        font-family:"sans-serif";
    }
    .latter-content .black-content{
        margin-left: 24rem;
        height: 6rem;
        font-size: 3rem;
    }
    .orange-square{
        height: 25rem;
        width: 25rem;
        background-color:#da9b01;
        padding: 1rem;
        margin-left: 2rem;
    }
    .orange-square p{
        transform: rotate(-1deg)
    }
    .footerContainer{
        grid-area: footer;
        display: flex;
        align-items: center;
        background-color: #150937;
        color: #eae6db;
        padding-left: 1rem;
    }
</style>
<div class="headerContainer">
    <div class="left-header">
        <div class="logo">
            <svg viewBox="0 0 1 1">
                <polygon points="0.1,0.1 0.1,0.9 0.9,0.9 0.9,0.1"></polygon>
            </svg>
        </div>
        <div class="logoName"><p>QWERik9</p></div>
    </div>
    <div class="right-header">
        <a href="https://github.com/erikstankevich">Projects</a>
    </div>
</div>
<div class="contentContainer">
    <div class="first-content">
        <p><code>01001000 01101001</code></p>
    </div>
    <div class="blue-content">
        <p>Herzlich Willkommen!</p>
    </div>
    <div class="black-content" id="upper-black">
        <p>Salut!</p>
    </div>
    <div class="latter-content">
        <div class="red-content">
            <p>Привет!</p>
        </div>
        <div class="black-content">
            <p>Hello!</p>
        </div>
    </div>
</div>
<div class="orangeContainer">
    <div class="orange-square">
        <p><code>
            This is my home page. <strong>Welcome</strong>. (I've created it on June 2nd 2025.) <br> <br>
            I consider this to be my first <em>real</em> website.
            <br><br>
            There is no specific goal in mind - well, I just want <em>it</em> to become a habit.
            <br><br>
            By <em>it</em> I mean studying, be it programming/scripting/devloping/... 
            or something completely unrelated, like learning an actual language.
            <br><br>
            The lines are to blurry, all I know is, <strong>I love</strong> tech. Software AND <strong>Hardware</strong>. 
            <br><br>
            Currently I want to learn more about network administration,
            I feel like it is totally overlooked. 
            Well, it certainly was not on <em>my</em> radar, until recently.

        </code></p>
    </div>
</div>
<div class="footerContainer">
    <p>About</p>
</div>
    