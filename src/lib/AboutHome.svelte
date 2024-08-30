<div class="bg">
    <div class="left">
        <img class="image" src="https://live.staticflickr.com/65535/53468982674_63a3e7f0de_b.jpg" />
    </div>
    <div class="right">
        <h1>About us</h1>
        <p>
            We are a FIRST Tech Challenge (FTC) team made up of 7 members from
            Richland High School, in Eastern Washington.
            We design, build, program, and compete robots in the FTC
            competition.
        </p>
    </div>
</div>
<div class="bg">
    <!-- <div class="image">
         <!-- <img src="Robot.png" alt="Our team" class="picture"> -->
    <!-- </div> --> -->
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
        width: 50%;
        margin-right: 5vw;
    }
    .image {
        background-color: hsl(0 0% 14%);
        width: 90%;
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
