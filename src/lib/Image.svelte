<script>
 export let src;
 export let alt;
</script>


<img id="image" {src} {alt}>

<style>
    #image {
        background-color: var(--bg-color);
        width: 90%;
        border-radius: 9px;
        box-shadow: 0 0 15px var(--secondary-bg-color);
    }
</style>
