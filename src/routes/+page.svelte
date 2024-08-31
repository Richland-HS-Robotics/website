<script>
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte";
    import CarouselSection from "$lib/CarouselSection.svelte";
    import Welcome from "../lib/Welcome.svelte";
    import About from "../lib/AboutHome.svelte";
    import Tabs from "../lib/tabs/Tabs.svelte";
    import Sponsors from "../lib/Sponsors.svelte";

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
    <About />

    <Sponsors />
    <Tabs items={items} >
        <div slot="body1">
            <h2>Student at Richland High School</h2>


            <p>Come to one of our club meetings, or attend one of our events.</p>
        </div>

        <div slot="body2">
            <h2>Potential Sponsor</h2>

            <p>
                You can donate to us at our <a
                href="https://secure.givelively.org/donate/washington-first-robotics/tyler-bartlett-3">Donation
                Page</a> , or email us about it at <a
                href="mailto:contact@rhs-robotics.com">contact@rhs-robotics.com</a>
            </p>
            <p>
                Your donation would help us pay our team fees, buy necessary
                robot parts, cover transportation costs, and be prepared for any
                other unexpected costs.
            </p>

            <p>
                To thank you we would love to put your name or logo on our
                robot, robot cart, and portfolio.
            </p>
        </div>

        <div slot="body3">
            <h2>Potential Coach</h2>

            <p>
                We are always looking for more coaches and mentors. Contact us at
                <a href="mailto:contact@rhs-robotics.com">contact@rhs-robotics.com</a>
            </p>

        </div>
    </Tabs>
</div>
