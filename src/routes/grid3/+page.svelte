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
        background-color: #f3f3f3;
        font-family: Arial;
    }

    .headerContainer{
        grid-area: header;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-areas: "left right";
        background-color: #000; 
        color: white;
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
    }
    .red-content{
        height: 3rem;
        width: 6rem;
        display:flex;
        align-items: center;
        justify-content: center;
        padding: 10px;
        background-color:red;
        color: white;
    }
    .orangeContainer{
        padding: 1rem;
        padding-right: 2rem;
        grid-area: orange;
        display: grid;
        align-items: end;
        justify-content: end;
    }
    .orange-square{
        height: 20rem;
        width: 20rem;
        background-color:orange;
    }
    .footerContainer{
        grid-area: footer;
        display: flex;
        align-items: center;
        background-color: #008;
        color: white;
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
        <p>About</p>
        <p>Blog</p>
    </div>
</div>
<div class="contentContainer">
    <div class="red-content">
        <p>Content</p>
    </div>
</div>
<div class="orangeContainer">
    <div class="orange-square"></div>
</div>
<div class="footerContainer">
    <p>About</p>
</div>
    