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
        "Education Education"
        "Work Work";
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
        border: 2px solid #fff;
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
    textarea{
        all:unset;
        padding: 1rem;
        background-color: #fff;
        border-radius: 2px;
        white-space: pre-wrap;
        font-size: 0.9rem;
    }
    .Work{
        grid-area: Work;
        display: grid;
    }
    .Work button{
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
    <div class="Work">
        <p>Work</p>
        <textarea rows="9" placeholder=
"Job Title:
Detective
Company:
NYPD
Start Date:
1988
End Date:
1999
Job Responsilities:
Keep Neighbour save"
        ></textarea>
        <button>Send</button>
    </div>
</div>