<div class="bg">
    <div class="left">
        <h1>About us</h1>
        <p>
            We are a FIRST Tech Challenge (FTC) team made up of 7 members from
            Richland High School, in Eastern Washington.
        </p>
    </div>
    <div class="right">
        <p>
            We design, build, program, and compete robots in the FTC
            competition.
        </p>
    </div>
</div>
<div class="bg">
    <div class="image">
        <img src="Robot.png" alt="Our team" class="picture">
    </div>
</div>

<link
    href="https://fonts.googleapis.com/css?family=Open+Sans"
    rel="stylesheet"
/>

<style>
    .bg {
        background-color: var(--bg-color);
        width: 100%;
        display: flex;
    }
    .left {
        width: 40vw;
        margin-left: 5vw;
    }
    h1 {
        color: var(--text-color);
    }
    p {
        color: var(--text-color);
    }
    .right {
        width: 40vw;
        padding-top: 300px;
        margin-left: 10vw;
        padding-bottom: 100px;
    }
    .image {
        background-color: hsl(0 0% 14%);
        width: 90%;
        margin-left: 5vw;
        margin-bottom: 100px;
        border-radius: 7px;
    }
    .picture{
        width: 100%;
        height: auto;
    }
    @media only screen and (max-width: 768px) {
        .left{
            width: 90vw;
        }
        .bg{
            flex-direction: column;
            padding-top: 50px;
        }
    }
</style>
