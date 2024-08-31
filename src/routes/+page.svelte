<script>
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte";
    import CarouselSection from "$lib/CarouselSection.svelte";
    import Welcome from "../lib/Welcome.svelte";
    import About from "../lib/AboutHome.svelte";
    import Tab1 from "../lib/Tab1.svelte";
    import Tab2 from "../lib/Tab2.svelte";
    import Tab3 from "../lib/Tab3.svelte";
    import Tabs from "../lib/Tabs.svelte";
    import Sponsors from "../lib/Sponsors.svelte";

    let count = 0;

    let items = [
        { label: "Content", value: 1, component: Tab1 },
        { label: "Interactions", value: 2, component: Tab2 },
        { label: "Tab 3", value: 3, component: Tab3 },
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
    <Tabs {items} />
</div>
