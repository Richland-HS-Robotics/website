
<script>
 import Header from "$lib/Header.svelte";
 import Footer from "$lib/Footer.svelte";
</script>

<div class="box">
    <Header class="row header" />


    <div id="slot" class="row content">
        <slot />
    </div>

    <Footer class="row footer" />
</div>


<style>
 #slot{
     margin-left: 5vw;
 }
</style>
