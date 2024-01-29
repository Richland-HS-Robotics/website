<script>
 import Header from "$lib/Header.svelte";
 import Footer from "$lib/Footer.svelte";
 import CarouselSection from "$lib/CarouselSection.svelte";

 let count = 0;
</script>


<Header/>


<div id="main">

    <CarouselSection />

</div>

<Footer/>


<style>
 #main{
     width:70%;
     margin: 0 auto;
     justify-content: center;
 }
</style>
