<style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
:global(body){
    height: 100vh;
    margin: 0;
    display: grid;
    grid-template-columns: auto;    
    font-family: 'EB Garamond';
    justify-content: center;
    align-content: center;
    background-color: grey;

}
.Card{
    padding: 1rem;
    padding-bottom: 0.6rem;
    height: 11rem;
    width: 19rem;
    background-color: #eae6db;
    box-shadow: 0 2px 2px  rgba(0, 0, 0, 0.5);
    display: grid;
    grid-template-areas: 
    "Head"
    "Center"
    "Tail";
    align-content: space-between;
}
.Head{
    grid-area: Head;
    display: flex;
    justify-content: space-between;
    font-size: 0.8rem;

}
.Head a{
    all: unset;
    cursor: pointer;
}
#at{
    display: flex;
    justify-content: center;
    align-content: center;
    font-size: 0.6rem;
}
.Center{
    grid-area: Center;
    display: grid;
    justify-content: center;
    align-content: center;
}
#Center-head{
    font-size: 1.1rem;
    display: flex;
    justify-content: center;
}
#Center-tail{
    display: flex;
    justify-content: center;
    font-size: 0.8rem;
}
.Tail{
    grid-area: Tail;
    display: flex;
    justify-content: space-around;
    font-size: 0.6rem;
}
</style>
<div class="Card">
    <div class="Head">
        <div class="Left-Head">
            <p>21estankevich</p>
            <p id="at">@gmail.com</p>
        </div>
        <div class="Right-Head">
            <a href="https://github.com/erikstankevich">Github</a>
        </div>
    </div>
    <div class="Center">
        <p id="Center-head">Erik Sokolov</p>
        <p id="Center-tail">Network Engineer</p>
    </div>
    <div class="Tail">
        <p>Carl-von-Ossietky Str. 54, 65197 Wiesbaden</p>
    </div>
</div>

<link href="https://fonts.googleapis.com/css2?family=EB+Garamond&display=swap" rel="stylesheet">
