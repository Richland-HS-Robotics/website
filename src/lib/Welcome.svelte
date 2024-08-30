<link
    href="https://fonts.googleapis.com/css?family=Open+Sans"
    rel="stylesheet"
/>

<div class="gradient">
    <div class="text">
        <h1>RHS Robotics</h1>
        <p>
            We design, build, program, and compete robots in the FTC
            competition.
        </p>
        <button class="button">Learn more</button>
    </div>
    <div class="image">
        <img src="Robot.png" alt="Our robot" class="robot" />
    </div>
    <svg width="50vw" height="50vw">
  <circle cx="25vw" cy="25vw" r="25vw" fill="#4e5565" />
</svg>
</div>

<style>
    svg{
        position: absolute;
        top: -25px;
        left: 45vw;
        z-index: 0;
        filter: blur(150px);
    }
    .text {
        padding-top: 150px;
        font-family: "Open Sans", sans-serif;
        color: var(--text-color);
        margin-left: 5vw;
        width: 40vw;
    }
    .gradient {
        /*background:
            linear-gradient(to top left, #1c1c1c, rgba(32, 33, 36, 0), #121212),
            linear-gradient(to top right, #1c1c1c, rgba(32, 33, 36, 0), #4e5565)
                rgb(32, 33, 36);*/
        background-color: var(--bg-color);
        position: relative;
        width: 100%;
        z-index: 0;
        display: flex;
        margin-top: -100px;
    }
    h1 {
        color: var(--text-color);
    }
    .button {
        margin-top: 25px;
    }
    .image {
        width: 60vw;
        margin-right: 5vw;
        z-index: 1;
    }
    .robot {
        width: 100%;
        margin-top: 100px;
    }
    @media only screen and (max-width: 768px) {
        .image {
            width: 90vw;
            margin-left: 5vw;
        }
        .text {
            width: 90vw;
            padding-top: 25px;
        }
        .gradient {
            flex-direction: column;
        }
        .gradient > * {
            order: 1;
        }
        .image {
            order: 0;
        }
    }
</style>
