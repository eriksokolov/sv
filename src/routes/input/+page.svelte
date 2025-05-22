<script>
    let name = "Foo Bar";
    let email = "foobar@mail.com";
    let phone = "0982734980";

</script>
<style>
:global(body){
    padding:0;
    margin:0;
}
.main-container{
    display: grid;
    grid-template-columns: 3fr 1.5fr;
    height: 100vh;
}
.left-container{
    background-color: grey;
    display: flex;
    align-content: center;
    justify-content: center;

}
.page{
    margin: 1rem;
    padding: 20rem 15rem;
    background-color: white;
}
.head-container{
    background-color: blue;
    color: white;
}

.right-container{
    padding: 3rem 4rem;
}


</style>

<div class="main-container">
    <div class="left-container">
        <div class="page">
            <div class="head-container">
            <p>{name}</p>
            <p>{email}</p>
            <p>{phone}</p>
            </div>
        </div>
    </div>

    <div class ="right-container">
        <div class="general-container">
            <p>General information</p>
            <input placeholder="name">
            <input placeholder="email">
            <input placeholder="phone">
        </div>
        <div class="education-container">
            <p>Education</p>
            <input placeholder="school">
            <input placeholder="degree">
            <input placeholder="date">
        </div>
        <div class="practical-container">
            <p>practical experience</p>
            <input placeholder="company">
            <input placeholder="position">
            <input placeholder="date">
        </div>
    </div>
</div>