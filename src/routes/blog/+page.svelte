<style>
    div {
        display: block;
        unicode-bidi: isolate;
    }
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    .left-container{
        background-color: #ff3;
        padding: 3rem 4rem;
        position: relative;
        height: 100%;
    }
    .right-container{
        background-color: #f39;
        padding: 3rem 4rem;
        display: grid;
        grid-template-columns: 3fr 1.5fr;

    }
    .main-container{
        height: 100vh;
        display: grid;
        width: 100%;
        grid-template-columns: 3fr 1.5fr;
        position: relative;
    }
    .lorem-container{
        border: 2px solid grey;
        padding: 1rem;
        position: relative;
    }

</style>

<div class ="main-container">
    <div class="left-container">
        <h1>Blog Index</h1>

        <ul>
            <li>
            <a href="/blog/post1">Post 1</a>
            </li>
            <li>
            <a href="/blog/post2">Post 2</a>
            </li>
        </ul>
    </div>
    <div class= "right-container">
        <div class="lorem-container">
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Beatae, quas? Nam obcaecati, eius ab culpa saepe enim exercitationem? Vitae suscipit vero modi veritatis ab, sed nulla tenetur aut adipisci facere!</p>
        </div>
        <div class="image-contianer">
            <img src="/favicon.png" alt="favicon">
        </div>
    </div>
</div>