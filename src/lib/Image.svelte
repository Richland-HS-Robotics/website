<script>
import Img from '@zerodevx/svelte-img';

 /* import team_pic from "$lib/../assets/Team-picture.jpg?as=run"; */

 export let src;
 export let alt;
</script>


<Img class="optimized-image" src="{src}" {alt} />

<style>
    :global(.optimized-image) {
        background-color: var(--bg-color);
        width: 90%;
        height: auto;
        border-radius: 9px;
        box-shadow: 0 0 15px var(--secondary-bg-color);
    }
</style>
