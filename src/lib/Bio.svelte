
<script>
 export let roles = ["GenericRole"];
 export let name = "GenericPerson";
 export let src = "favicon.png";
 export let reversed = false;
</script>


<div id="container">
    {#if !reversed}
        <img {src} />
    {/if}
    <div>
        <div id="header" class="p">
            <h3>{name}</h3>
            <div>
                {#each roles as role}
                    <span>{role}</span>
                {/each}
            </div>
        </div>
        <p class="p">
            <slot />
        </p>
    </div>
    {#if reversed}
        <img {src} />
    {/if}
</div>



<style>
 #container{
     width: 100%;
     display: flex;
     align-items: center;
     justify-content: space-between;
     padding: 1.5em;
     border-radius: 1.5em 1.5em;

     background-color: #ffff4d;

     /* border: solid 2px black; */
     box-shadow: 10px 10px grey;
 }

 #header{
     display: flex;
     justify-content: space-between;
     align-items: center;
 }

 img{
     height: auto;
     max-width: 25%;
     display: flex;
     margin-right: 3em;
     border-radius: 0.7em 0.7em;
 }

 .p{
     width: 70%;
 }

 p{
     text-align: justify;
 }

 span{
     font-size: 1.3em;
     background-color: #4d79ff;
     padding: 0.2em;
     border-radius: 0.4em 0.4em;
     margin-left: 0.1em;
     margin-right: 0.1em;
 }
</style>
