<script>
 import Header from "$lib/Header.svelte";
 import Footer from "$lib/Footer.svelte";
 import CarouselSection from "$lib/CarouselSection.svelte";
 import Banner from "$lib/Banner.svelte";

 let count = 0;
</script>




<Banner />

<div id="main">
    <h2>A heading</h2>
    <br/>
    <br/>
    <br/>
    <br/>
    A headingA heading<br/>


    <CarouselSection />

</div>



<style>
 #main{
     width:70%;
     margin: 0 auto;
     justify-content: center;
 }
</style>
