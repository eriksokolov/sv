<style>
    :global(body){
        font-family: sans-serif;
        font-size: 16px;
        height: 100vh;

        display:grid;
        grid-template-areas:
        'header header header'
        'nav content sidebar'
        'nav footer footer';
        grid-template-columns: 1fr 4fr 1fr;
        grid-template-rows: 80px 1fr 80px;
    }

    .headerContainer,
    .footerContainer,
    .mainContainer,
    .asideContainer,
    .navContainer {
        background-color: steelblue;
        color: #fff;
        padding:20px;
        border: skyblue 1px solid;
    }
    .headerContainer{
        grid-area: header;
    }
    .footerContainer{
        grid-area: footer;
    }
    .mainContainer{
        grid-area: content;
    }
    .navContainer{
        grid-area:nav;
    }
    .asideContainer{
        grid-area:sidebar;
    }
</style>
<div class="headerContainer">header</div>
<div class="footerContainer">footer</div>
<div class="mainContainer">main</div>
<div class="asideContainer">aside</div>
<div class="navContainer">nav</div>