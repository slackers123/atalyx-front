<script>
import TeamMember from "$lib/TeamMember.svelte";

</script>
<div class="content">
    <div class="team">
        <h1>Meet The Team</h1>
        <p>Atalyx Games is an independent Game Studio in Austria Vienna with the <br>
            founders being Toby Kogler, Aaron Hager and Boris Kostadinov. We focus on <br>
            creating new, unique experiences for our audience. </p>

        <div class="rows">
            <div class="r1">
                <TeamMember src={"Toby Kogler.png"} name={"Toby Kogler"} roles={["General Director", "Composer"]}/>
                <TeamMember src={"Aaron Hager.png"} name={"Aaron Hager"} roles={["2D/3D-Artist", "Level-Designer"]}/>
                <TeamMember src={"Lewin Strobl.png"} name={"Lewin Strobl"} roles={["2D/3D-Artist"]}/>
            </div>
            <div class="r2">
                <TeamMember src={"Boris Kostadinov.png"} name={"Boris Kostadinov"} roles={["Programmer"]}/>
                <TeamMember src={"Severin Gebesmair.png"} name={"Severin Gebesmair"} roles={["Programmer", "Sound-Design"]}/>
            </div>
            <img class="award" src="award.png" alt="Award">
        </div>
    </div>
</div>


<style>

    .award {
        padding-top: 10rem;
    }

    .rows {
        text-align: center;
        padding-left: 2rem;
        padding-right: 2rem;
    }

    .r1, .r2 {
        padding-top: 2rem;
        display: flex;
        justify-content: space-evenly;
    }

    .content {
        background-image: url('sc1.png');
        background-repeat: no-repeat;
        background-attachment: fixed;
        background-size: cover;
        height: 150vh;
        z-index: 4;
    }

    .team {
        height: 135vh;
        margin-left: 20vw;
        margin-right: 20vw;
        padding: 5vw;
        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        background-color: white;
    }
</style>