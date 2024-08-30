<svelte:head>
    <title>RHS Robotics Homepage</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</svelte:head>

<script>
 import Header from "$lib/Header.svelte";
 import Footer from "$lib/Footer.svelte";
 import CarouselSection from "$lib/CarouselSection.svelte";
 import FTC from "$lib/FTC.svelte";
 import Welcome from "../lib/Welcome.svelte";
 import About from "../lib/AboutHome.svelte";
    import Robots from "../lib/Robots.svelte";
import Sponsors from "../lib/Sponsors.svelte";


 let count = 0;
 </script>



 <!-- <Banner /> -->

<div id="main">
<Welcome />
    <About />


    <FTC />
    <Robots />
    <Sponsors />
</div>




