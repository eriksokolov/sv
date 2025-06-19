<style>
    *{
        margin:0;
        padding:0;
        box-sizing: border-box;
    }
    :global(body){
        margin:0;
        height: 300vh;
        background-color: rgb(90,90,90);
        display:grid;
        justify-content: center;
        align-content: center;
    }
    .paper{
        transform: scale(1);
        margin: 1rem;
        padding: 5rem;
        height: 75rem;
        width: 50rem;
        background-color: #eae6db;
        box-shadow: 3px 3px 3px rgba(0,0,0, 0.5);
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 0fr 0fr 0fr;
        grid-template-areas:
        "title title"
        "P-Portrait P-Portrait"
        "Education Education";
        justify-content: space-between;
        align-items: start;
    }
    .paper *{
        margin-bottom: 1rem;
    }
    #portrait{
        justify-self: end;
        height: 12rem;
        width: 12rem;
        border-radius: 9rem;
        box-shadow: 1px 15px 9px rgba(0,0,0, 0.5)
    }
    .P-Portrait{
        grid-area: P-Portrait;
        display: grid;
        grid-template-columns: 1fr 1fr;
        justify-items: space-between;
        align-items: center;
    }
    .Education{
        grid-area: Education;
        display: grid;
    }
    .P-Portrait > div {
        display: grid;
    }
    button{
       justify-self: start; 
    }
    .Education button {
        align-self: flex-start;
    }





</style>
<div class="paper">
    <p class="title"><strong>CV</strong></p>
    <div class="P-Portrait">
        <div>
            <p>Personal information</p>
            <textarea rows=9 placeholder=
"Full name:
Max Payne
Email:
payne@nypd.org
Phone:
+1838383838
Address:
Sherman Oaks"
            ></textarea>
            <button>Send</button>
        </div>
        <img id="portrait" src="/Max_Payne_Image.png" alt="Portrait">
    </div>
    <div class="Education">
        <p>Education</p>
        <textarea  rows=9 placeholder=
"Degree:
The Bachelor
Institution:
NYPD
Completion Date:
1999"></textarea>
        <button>Send</button>
    </div>
</div>