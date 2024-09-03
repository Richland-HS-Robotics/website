<script>
    import SideBySide from "$lib/SideBySide.svelte";
    import Image from "$lib/Image.svelte";
</script>

<svelte:head>
    <title>Richland Robotics - Robots</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
</svelte:head>

<h1 id="robots">Meet our robots</h1>

<div class="large-card">
    <h2 id="robot">CenterStage - 15010</h2>
    <div class="flex">
        <img
            src="robot_hang.jpg"
            alt="Gold Team Centerstage robot"
            class="image"
        />
        <div class="text-container">
            <p id="robot-text">
                Our most successful robot yet, built for the 2023-2024
                CenterStage challenge. We focused on endgame tasks and
                autonomous, achieving 5th place in the interleague tournament.
                We were picked by team #11990 RUN KANO for the playoffs and won
                the final match.
            </p>
        </div>
    </div>
</div>

<div class="large-card-right">
    <h2 id="robot">PowerPlay - 18249</h2>
    <div class="flex-right">
        <div class="text-container">
            <p id="robot-text">
                Our junior team #18429 built a robot for the 2022-2023 PowerPlay
                challenge and outperformed the main team. They achieved 9th
                place in the qualification matches and were picked by team
                #11990 RUN KANO for the playoffs. The alliance won the semifinal
                but lost in the finals to teams #8099 and #19589.
            </p>
        </div>
        <img
            src="/robots/Gold-team-powerplay.png"
            alt="Gold Team PowerPlay robot"
            class="image-right"
        />
    </div>
</div>

<div class="large-card">
    <h2 id="robot">PowerPlay - 15010</h2>
    <div class="flex">
        <img
            src="/robots/Green-team-powerplay.jpg"
            alt="Green Team PowerPlay robot"
            class="image"
        />
        <div class="text-container">
            <p id="robot-text">
                Our robot for the 2022-2023 POWERPLAY challenge faced electrical
                and connection issues. We performed decently in the first two
                league meets but struggled in the interleague tournament,
                finishing in 14th place.
            </p>
        </div>
    </div>
</div>

<div class="large-card-right">
    <h2 id="robot">Freight Frenzy - 15010</h2>
    <div class="flex-right">
        <div class="text-container" id="right-text">
            <p id="robot-text">
                Our junior team #18429 built a robot for the 2022-2023 PowerPlay
                challenge and outperformed the main team. They achieved 9th
                place in the qualification matches and were picked by team
                #11990 RUN KANO for the playoffs. The alliance won the semifinal
                but lost in the finals to teams #8099 and #19589.
            </p>
        </div>
        <img
            src="/robots/Green-team-freight-frenzy.jpg"
            alt="Green Team Freight Frenzy robot"
            class="image-right"
        />
    </div>
</div>

<!--
<SideBySide>
    <Image
        slot="right"
        src="/robot_hang.jpg"
        alt="Our Gold Team Centerstage Robot"
    />

    <div slot="left">
        <h2>CENTERSTAGE - 15010</h2>

        <p>
            This is the robot that we built for the 2023-2024 CENTERSTAGE
            challenge. It is our most successful robot yet.
        </p>

        <br />

        <p>
            We never really achieved a good design for the pixel intake and
            outtake, so this season we really focused on the endgame tasks, as
            well as the autonomous section. Together, our excellent endgame and
            autonomous got us to 5th place in the qualification rounds of our
            interleague tournament. For the playoff, we convinced team #11990
            RUN KANO to pick us entirely because of our autonomous and endgame.
            Together, our alliance won our semifinal, and then went on to win
            the final in an exciting final match.
        </p>

        <br />

        <p>
            Unfortunately, only three teams were set to advance from our region,
            so we were unable to advance to state.
        </p>

        <br />

        <h3>Awards</h3>
        <ul>
            <li>5th place in quals</li>
            <li>Winning Alliance 1st Pick</li>
            <li>Innovate Award Winner</li>
        </ul>
    </div>
</SideBySide>

<SideBySide>
    <Image
        slot="left"
        src="/robots/Gold-team-powerplay.png"
        alt="Our gold team powerplay robot"
    />
    <div slot="right">
        <h2>POWERPLAY - 18249</h2>

        <p>
            This is the robot that our junior team #18429 built for the
            2022-2023 POWERPLAY challenge. Although they did not have nearly as
            many resources as the main team, they ended up outperforming them.
        </p>

        <br />

        <p>
            With this robot, we were able to achieve 9th place in the
            qualification matches, before being picked by team #11990 RUN KANO
            for the playoffs. Together our alliance won our semifinal, winning
            one of our matches by only 6 points! However, we were beaten in the
            finals by teams #8099 and #19589.
        </p>

        <br />

        <h3>Awards</h3>
        <ul>
            <li>9th place in quals</li>
            <li>Finalist Alliance 1st pick</li>
            <li>Connect Award Winner</li>
        </ul>
    </div>
</SideBySide>
<br />
<br />

<SideBySide>
    <Image
        slot="right"
        src="/robots/Green-team-powerplay.jpg"
        alt="Our green team powerplay robot"
    />
    <div slot="left">
        <h2>POWERPLAY - 15010</h2>

        <p>This is the robot we built for the 2022-2023 POWERPLAY challenge.</p>

        <br />

        <p>
            Unfortunately we suffered some electrical and co
            slot="right"nnection issues, so we did not do very well with this
            robot. We did decently for our first two league meets, but had
            issues for our interleague tournament and ended up down in 14th
            place.
        </p>

        <br />

        <h3>Awards</h3>
        <ul>
            <li>14th place in quals</li>
            <li>Innovate Award Winner</li>
        </ul>
    </div>
</SideBySide>

<br />
<br />

<SideBySide>
    <Image
        slot="left"
        src="/robots/Green-team-freight-frenzy.jpg"
        alt="Our green team freight frenzy robot"
    />
    <div slot="right">
        <h2>Freight Frenzy - 15010</h2>

        <h3>Awards</h3>
        <ul>
            <li>5th place in quals</li>
            <li>Think Award Winner</li>
        </ul>
    </div>
</SideBySide>-->

<style>
    #robots {
        padding-top: 80px;
        padding-bottom: 50px;
        font-size: 60px;
        font-weight: bold;
    }
    .large-card {
        width: 75vw;
        border: 1px solid var(--yellow);
        border-radius: 7px;
        background-color: var(--secondary-bg-color);
        box-shadow: 0 0 15px var(--secondary-bg-color);
        margin-bottom: 75px;
    }
    .large-card-right {
        width: 75vw;
        border: 1px solid var(--yellow);
        border-radius: 7px;
        background-color: var(--secondary-bg-color);
        box-shadow: 0 0 15px var(--secondary-bg-color);
        margin-left: 15vw;
        margin-bottom: 75px;
    }
    #robot {
        text-align: center;
        padding-top: 50px;
        font-size: 50px;
        margin-bottom: 20px;
    }
    .flex {
        width: 70vw;
        margin-left: 2.5vw;
        margin-right: 2.5vw;
        display: flex;
    }
    .flex-right {
        width: 70vw;
        margin-left: 2.5vw;
        margin-right: 2.5vw;
        display: flex;
        justify-content: flex-end;
    }
    .image {
        width: 20vw;
        height: auto;
        border-radius: 7px;
        box-shadow: 0 0 15px var(--bg-color);
        display: flex;
        margin-right: 2.5vw;
        margin-bottom: 2.5vw;
    }
    .image-right {
        width: 20vw;
        height: auto;
        border-radius: 7px;
        box-shadow: 0 0 15px var(--bg-color);
        display: flex;
        margin-left: 2.5vw;
        margin-bottom: 2.5vw;
    }
    #robot-text {
        width: 100%;
    }
    .text-container {
        width: 42.5vw;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
  @media screen and (max-width: 736px) {
    .flex, .flex-right{
        margin-right: 5vw;
        margin-left: 5vw;
    }
    #robot{
        font-size: 40px;
        max-width: 80vw;
        text-align: left;
        margin-left: 5vw;
    }
    .large-card, .large-card-right{
        width: 90vw;
        margin-left: 0;
    }
    .flex, .flex-right{
        flex-direction: column;
    }
    .flex-right{
        flex-direction: column-reverse;
    }
    .image{
        width: 80vw;
    }
    .image-right{
        width: 80vw;
        margin: 0;
    }
    .text-container{
        width: 80vw;
        margin-top: 25px;
        margin-bottom: 2.5vw;
    }
  }
</style>
