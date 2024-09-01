<script>
 import Carousel from "svelte-carousel";
 import {browser} from "$app/environment";

 let carousel;

 const handleNextClick = () =>{
     carousel.goToNext();
 }
</script>


{#if browser}
    <Carousel bind:this={carousel}
              autoplay
              autoplayDuration={5000}
              autoplayProgressVisible
              pauseOnFocus
    >
        <div slot="prev" let:showPrevPage on:click={showPrevPage} class="custom-arrow custom-arrow-prev">
            <i />
        </div>

        {#each {length:10} as _, index}
            <img src="https://picsum.photos/seed/{index + 1}/1920/1080" alt="A placeholder image" />
        {/each}

        <div slot="next" let:showNextPage on:click={showNextPage} class="custom-arrow custom-arrow-next" role="button" on:keydown={showNextPage} tabindex="0">
            <i />
        </div>

    </Carousel>
{/if}



<style>
 .custom-arrow{
     width:20px;
     opacity: 0.4;
     position: absolute;
     top: 0;
     bottom: 0;
     z-index: 1;
     transition: opacity 150ms ease;
     display: flex;
     align-items: center;
     cursor: pointer;
     background-color: #000000;
 }

 .custom-arrow-next{
     right:0;
 }

 .custom-arrow-prev{
     left:0;
 }

 .custom-arrow>i{
     z-index: 30;
     border: solid #ff0000;
     border-width: 0 5px 5px 0;
     padding: 5px;
     position: relative;
     opacity: 1;
 }

 .custom-arrow-next>i{
     transform: rotate(-45deg);
     left: -4px;
 }

 .custom-arrow-prev>i{
     transform: rotate(135deg);
     right: -4px;
 }
</style>
