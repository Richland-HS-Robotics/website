<script>
 import CarouselSection from "../lib/CarouselSection.svelte";

 let tabs = [
     {name: "Hello", comp: CarouselSection},
     {name: "Goodbye", comp: false},
 ];

 let cur = tabs[0];

</script>

{#each tabs as tab}
    <button class:selected={cur === tab} on:click={() => (cur = tab)}>
        {tab.name}
    </button>
{/each}

<main>
    <svelte:component this={cur.comp} />
</main>
