<script>
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte";
    import Welcome from "../lib/Welcome.svelte";
    import SideBySide from "../lib/SideBySide.svelte";
    import Tabs from "../lib/tabs/Tabs.svelte";
    import Sponsors from "../lib/Sponsors.svelte";
    import Image from "../lib/Image.svelte";

    import teamPicture from "$lib/../assets/Team-picture.jpg?as=run";

    let count = 0;

    let items = [
        { label: "Student", value: 1 },
        { label: "Sponsor", value: 2 },
        { label: "Coach", value: 3 },
    ];
</script>

<svelte:head>
    <title>Richland Robotics - Home</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
</svelte:head>

<!-- <Banner /> -->

<div id="main">
    <Welcome />
    <SideBySide>
        <Image class="image" slot="left" alt="Our team" src={teamPicture} />
        <div slot="right">
            <h2>About us</h2>
            <p>
                We are a <a href="https://www.firstinspires.org/robotics/ftc">
                    FIRST Tech Challenge (FTC)</a
                >
                team made up of 7 members from
                <a href="https://richland.rsd.edu/">Richland High School</a>, in
                Eastern Washington. We design, build, program, and compete
                robots in the FTC competition.
            </p>
        </div>
    </SideBySide>

    <h2 id="if">Get involved</h2>
    <div id="container">
        <div class="card">
            <div class="heading-div">
                <span class="fa-brands fa-google-scholar icon" id="icons"
                ></span>
                <span class="heading">Student</span>
            </div>
            <span class="contact">
                <p>
                    Come to one of our club meetings, or attend one of our
                    events.
                </p>
            </span>
            <a class="button" href="/involved">Learn more</a>
        </div>
        <div class="card">
            <div class="heading-div">
                <span class="fa-solid fa-heart icon" id="icons"></span>
                <span class="heading">Sponsor</span>
            </div>

            <span class="contact">
                <p>
                    You can donate to us at our <a
                        href="https://secure.givelively.org/donate/washington-first-robotics/tyler-bartlett-3"
                        >Donation Page</a
                    >, or email us about it at
                    <a href="mailto:contact@rhs-robotics.com"
                        >contact@rhs-robotics.com</a
                    >
                </p>
            </span>
            <a class="button" href="/involved">Learn more</a>
        </div>
        <div class="card">
            <div class="heading-div">
                <span class="fa-solid fa-user-group icon" id="icons"></span>
                <span class="heading">Coach</span>
            </div>

            <span class="contact">
                <p>We are always looking for more coaches and mentors.</p>
            </span>
            <a class="button" href="/involved">Learn more</a>
        </div>
    </div>

    <!-- <Sponsors /> -->
    <!-- <Tabs items={items} >
         <div slot="body1">
         <h2>Student at Richland High School</h2>

         <p>Come to one of our club meetings, or attend one of our events.</p>
         </div>

         <div slot="body2">
         <h2>Potential Sponsor</h2>

         <p> You can donate to us at our <a
         href="https://secure.givelively.org/donate/washington-first-robotics/tyler-bartlett-3">Donation
         Page</a>, or email us about it at <a
         href="mailto:contact@rhs-robotics.com">contact@rhs-robotics.com</a>
         </p>

         <br/>

         <p> Your donation would help us pay our team fees, buy necessary
         robot parts, cover transportation costs, and be prepared for any
         other unexpected costs. </p>

         <br/>

         <p> To thank you we would love to put your name or logo on our
         robot, robot cart, and portfolio. </p>

         </div>

         <div slot="body3">
         <h2>Potential Coach</h2>

         <p> We are always looking for more coaches and mentors. Contact us
         at <a
         href="mailto:contact@rhs-robotics.com">contact@rhs-robotics.com</a>
         </p>

         </div>
         </Tabs> -->
</div>

<style>
    .button {
        margin-bottom: 2.5vw;
        margin-left: 2.5vw;
        text-decoration: none;
        color: var(--bg-color);
        position: relative;
        /* bottom: 2.5vw; */
        margin-top: auto;
        align-self: flex-start;
    }
    .button:hover {
        color: var(--secondary-bg-color);
    }
    #if {
        font-size: 50px;
        font-weight: bold;
        padding-top: 50px;
    }
    p {
        position: relative;
        z-index: 2;
    }
    #icons {
        margin-left: 2.5vw;
    }
    .icon {
        color: var(--text-color);
        font-size: 40px;
        /* margin-top: 5%; */
    }
    .heading-div {
        margin-top: 2.5vw;
        display: flex;
        flex-direction: column;
    }
    #container {
        display: flex;
        flex-direction: row;
        width: 90vw;
        background-color: var(--bg-color);
        margin-top: 50px;
    }
    .card {
        width: calc(90vw / 3 - 2vw);
        transform: translateX(-1vw);
        margin-left: 1vw;
        margin-right: 1vw;
        height: auto;
        border-radius: 7px;
        border: 1px solid var(--yellow);
        background-color: var(--secondary-bg-color);
        box-shadow: 0 0 15px var(--secondary-bg-color);
        display: flex;
        flex-direction: column;
    }
    a {
        text-decoration: underline;
    }
    a:hover {
        text-decoration: none;
        color: var(--text-color-hover);
    }
    .heading {
        font-size: 30px;
        /* margin-left: auto;
       margin-right: 25%; */
        display: block;
        color: var(--text-color);
        margin-left: 2.5vw;
        margin-top: 30px;
    }
    .contact {
        color: var(--text-color);
        font-size: 16px;
        display: block;
        margin-top: 5%;
        margin-left: 2.5vw;
        margin-bottom: 25px;
        width: calc(90vw / 3 - 7vw);
        flex-grow: 1;
    }
    @media screen and (max-width: 736px) {
        #container {
            flex-direction: column;
        }
        .card {
            width: 86vw;
            margin-bottom: 4vw;
            margin-top: 4vw;
        }
        .contact {
            margin-left: 5vw;
            width: 76vw;
            margin-bottom: 5vw;
            margin-right: 5vw;
        }
        #icons {
            margin-left: 5vw;
        }
        .heading {
            margin-left: 5vw;
        }
        p {
            padding-bottom: 25px;
        }
        .heading-div {
            margin-top: 5vw;
        }
    }
</style>
