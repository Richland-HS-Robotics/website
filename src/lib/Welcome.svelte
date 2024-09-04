<script>
    import Img from "@zerodevx/svelte-img";
    import team_pic from "$lib/../assets/Team-picture.jpg?as=run";
    import robot_render from "$lib/../assets/Robot_render.png?as=run";

</script>

<link
    href="https://fonts.googleapis.com/css?family=Open+Sans"
    rel="stylesheet"
/>

<div class="gradient">
    <div class="text">
        <h1>Richland Robotics</h1>
        <p>
            We design, build, program, and compete robots for the
            <a href="https://www.firstinspires.org/robotics/ftc"> FIRST Tech Challenge</a>.
        </p>
        <!-- <button class="button">Learn more</button> -->
    </div>
    <div class="image">
        <Img src={robot_render} alt="Our robot" class="robot" />
    </div>
    <svg width="50vw" height="50vw">
        <circle cx="25vw" cy="25vw" r="25vw" fill="#4e5565" />
    </svg>
</div>

<style>
    svg {
        position: absolute;
        top: -25px;
        left: 45vw;
        z-index: 1;
        filter: blur(150px);
    }
    .text {
        padding-top: 150px;
        font-family: "Open Sans", sans-serif;
        color: var(--text-color);
        margin-left: 0;
        width: 40vw;
        z-index: 2;
    }
    .gradient {
        /*background:
            linear-gradient(to top left, #1c1c1c, rgba(32, 33, 36, 0), #121212),
            linear-gradient(to top right, #1c1c1c, rgba(32, 33, 36, 0), #4e5565)
                rgb(32, 33, 36);*/
        background-color: var(--bg-color);
        width: 100%;
        z-index: 0;
        display: flex;
        margin-top: -70px;
    }
    .image {
        width: 60vw;
        margin-right: 5vw;
        z-index: 2;
        /* box-shadow: 0 0 8px 8px var(--bg-color) inset; */
    }
    :global(.robot) {
        width: 100%;
        height: auto;
        margin-top: 100px;
        background: none !important;
    }
    @media only screen and (max-width: 768px) {
        .image {
            width: 90vw;
            margin-left: 0;
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
