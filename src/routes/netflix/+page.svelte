<style>
    :root{
        --primary-color: #e50914;
    }
    :global(body){
        font-family: 'Arial';
        --webkit-font-smoothing: antialiased;
        background: #000;
        color: #999;
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }
    
    ul {
        list-style: none;
    }

    h1, h2, h3, h4 {
        color: #fff;
    }

    a {
        color: #fff;
        text-decoration: none;
    }

    p {
        margin: 0.5rem 0;
    }

    img {
        width: 100%;
    }

    .logo{
        position: absolute;
        width: 148px;
        height: 40px;
        background-color: red;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%)
    }

    .showcaseContainer{
        width: 100%;
        height: 93vh;
        position: relative;
        background: url('/backgroundNetflix.jpg') no-repeat center center/cover;
    }
    .showcaseContainer::after{
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 1;
        background: rgba(0,0,0,0.6); 
        box-shadow: inset 120px 100px 250px #000, inset -120px -100px 250px #000;

    }

    .showcase-topContainer{
        position: relative;
        height: 90px;
        z-index: 2;
    }
    .showcase-topContainer a {
        position: absolute;
        top: 50%;
        right: 0;
        transform: translate(-50, -50%);
    }
    a {
        display: inline-block;
        background: var(--primary-color);
        color: #fff;
        padding: 0.4rem 1.3rem;
        font-size: 1rem;
        text-align: center;
        border: none;
        cursor: pointer;
        margin-right: 0.5rem;
        outline: none;
        box-shadow: 0 1px 0 rgba(0,0,0,0.45);
    }
    .a-rounded{
        border-radius: 5px;
    }
    .a-xl {
        font-size: 2rem;
        padding: 1rem 2rem;
        text-transform: uppercase;
    }
    .showcase-contentContainer {
        position: relative;
        margin: auto;
        display: grid;
        justify-content: center;
        align-items: center;
        text-align: center;
        z-index: 2;
    }
    .showcase-contentContainer h1 {
        font-weight: 700px;
        font-size: 5.2rem;
        line-height: 1.1;
        margin: 0 0 1.5 0;
    }
    .showcase-contentContainer p {
        text-transform: uppercase;
        color: #fff;
        font-weight: 400;
        font-size: 1.9rem;
        line-height: 1.25;
        margin: 0 0 2rem;
    }


</style>
<div class="headContainer">
    <title>Neftlix - Watch TV Shows Online, Watch Movies Online</title>
    <div class="showcaseContainer">
        <div class="showcase-topContainer">
            <div class="logo"></div>
            <a href="#" class="a-rounded">Sign in</a>
        </div>
        <div class="showcase-contentContainer">
            <h1>See what's next</h1>
            <p>Watch anywhere. Cancel anytime</p>
            <a href="#" class="a-rounded a-xl">Watch Free For 30 Days</a>
        </div>
    </div>
</div>
<section class="tabs">
    <div class="container">
        <div id="tab-1" class="tab-item tab-border">
            <p class="hide-sm">Cancel Anytime</p>
        </div>
                <div id="tab-1" class="tab-item tab-border">
            <p class="hide-sm">Cancel Anytime</p>
        </div>
         <div id="tab-1" class="tab-item tab-border">
            <p class="hide-sm">Cancel Anytime</p>
        </div>
    </div>
</section>