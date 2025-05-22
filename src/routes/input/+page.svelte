<script>
    let name = "Name";
    let email = "Mail@mail.";
    let phone = "teleph0982734980";

    let school = "mguniversity"
    let degree = "degree of bachelor by ligma";
    let edudate = "date 24.24.2024";

    let company = "company usss"
    let position = "posiCBeDOtion"
    let pracdate = "25.25.2025 date"



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
}
.page{
    margin: 5rem;
    background-color: white;
    height: 200vh;
}
.head-container{
    display: flex;
    align-content: center;
    justify-content: center;
    background-color: darkblue;
    color: white;
    gap: 1rem;
}
.left-education{
    margin: 1rem;
}
.left-practical{
    margin: 1rem;
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
            <div class="left-education">
                <h2>education</h2>
                <p>{school}</p>
                <p>{degree}</p>
                <p>{edudate}</p>
            </div>
            <div class="left-practical">
                <h3>Practical Experience</h3>
                <p>{company}</p>
                <p>{position}</p>
                <p>{pracdate}</p>
            </div>

        </div>
    </div>

    <div class ="right-container">
        <div class="general-container">
            <p>General information</p>
            <input placeholder="name" bind:value={name}>
            <input placeholder="email" bind:value={email}>
            <input placeholder="phone" bind:value={phone}>
        </div>
        <div class="education-container">
            <p>Education</p>
            <input placeholder="school" bind:value={school}>
            <input placeholder="degree" bind:value={degree}>
            <input placeholder="date" bind:value={edudate}>
        </div>
        <div class="practical-container">
            <p>practical experience</p>
            <input placeholder="company" bind:value={company}>
            <input placeholder="position" bind:value={position}>
            <input placeholder="date" bind:value={pracdate}>
        </div>
    </div>
</div>