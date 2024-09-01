<script>
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte";
    import CarouselSection from "$lib/CarouselSection.svelte";
    import Welcome from "../lib/Welcome.svelte";
    import SideBySide from "../lib/SideBySide.svelte";
    import Tabs from "../lib/tabs/Tabs.svelte";
    import Sponsors from "../lib/Sponsors.svelte";
    import Image from "../lib/Image.svelte";

    let count = 0;

    let items = [
        { label: "Student", value: 1 },
        { label: "Sponsor", value: 2 },
        { label: "Coach", value: 3 },
    ];
</script>

<svelte:head>
    <title>RHS Robotics Homepage</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
</svelte:head>

<!-- <Banner /> -->

<div id="main">
    <Welcome />
    <SideBySide >
        <Image class="image"
               slot="left"
               alt="Our team"
               src="https://live.staticflickr.com/65535/53467755512_a217ccb400_h.jpg"
        />
        <div slot="right">
            <h1>About us</h1>
            <p>
                We are a <a href="https://www.firstinspires.org/robotics/ftc">
                FIRST Tech Challenge (FTC)</a> team made up of 7
                members from <a href="https://richland.rsd.edu/">Richland High
                School</a>, in Eastern Washington. We design, build, program,
                and compete robots in the FTC competition.
            </p>
        </div>
    </SideBySide>

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
