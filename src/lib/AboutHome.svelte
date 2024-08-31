<div class="bg">
    <div class="left">
        <img
            class="image"
            alt="Our team"
            src="https://live.staticflickr.com/65535/53468982674_63a3e7f0de_b.jpg"
        />
    </div>
    <div class="right">
        <h1>About us</h1>
        <p>
            We are a FIRST Tech Challenge (FTC) team made up of 7 members from
            Richland High School, in Eastern Washington. We design, build,
            program, and compete robots in the FTC competition.
        </p>
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
        padding-top: 25px;
        z-index: 0;
    }
    .left {
        width: 40vw;
        margin-left: 5vw;
        z-index: 2;
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
        z-index: 2;
    }
    .image {
        background-color: var(--bg-color);
        width: 90%;
        border-radius: 7px;
        box-shadow: 0 0 15px var(--secondary-bg-color);
    }
    @media only screen and (max-width: 768px) {
        .left {
            width: 90vw;
            order: 1;
        }
        .bg {
            flex-direction: column;
            padding-top: 50px;
        }
        .right {
            width: 90vw;
            margin-left: 5vw;
            margin-right: 0;
            order: 0;
        }
        .image{
            width: 90vw;
            padding-top: 50px;
        }
    }
</style>
