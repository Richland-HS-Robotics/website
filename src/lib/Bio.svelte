<script>
  import Modal from "$lib/Modal.svelte";

  export let roles = ["GenericRole"];
  export let name = "GenericPerson";
  export let src = "favicon.png";
  export let reversed = false;

  let showModal = false;

  let dialog;
</script>

<Modal bind:showModal>
  <div id="container">
    <img {src} class="dialogImg" />
    <div>
      <div id="header" class="p">
        <h3>{name}</h3>
        <div>
          {#each roles as role}
            <span class="role">{@html role}</span>
          {/each}
        </div>
      </div>
      <p class="p">
        <slot />
      </p>
    </div>
  </div>
</Modal>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<!-- svelte-ignore a11y-no-static-element-interactions -->
<div id="small-container" on:click={() => (showModal = true)}>
  <img {src} />
  <div>
    <span class="name">{name}</span>
    <ol>
      {#each roles as role}
        <li class="role">{@html role}</li>
      {/each}
    </ol>
  </div>
</div>

<!-- <button on:click={() => (showModal = true)}>Show modal</button> -->

<style>
  #small-container {
    /* width: 28em; */
    height: 20em;
    display: flex;
    justify-content: space-between;
    background-color: #f4f4f6;
    padding: 1.5em;
    cursor: pointer;
    transition: transform 0.2s ease-in-out;
}
#small-container:hover{
    transform: scale(1.03);
}

  #small-container > img {
    height: 100%;
  }

  .name {
    font-size: 1.5rem;
    font-weight: bold;
    margin-left: 0.5em;
    padding: 0.2em;
  }

  #container {
    /* max-width: 75%; */
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    /* padding: 1.5em; */
    /* border-radius: 1.5em 1.5em; */

    background-color: #f4f4f6;

    /* border: solid 2px black; */
    /* box-shadow: 5px 5px 5px #C7C7D1; */
    /*Shadow Color C7C7D1*/
  }

  /* dialog::backdrop{
    background: rgba(0,0,0,0.3);
    }
  */
  #header {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .dialogImg {
    height: auto;
    max-width: 25%;
    display: flex;
    margin-right: 3em;
  }

  .p {
    width: 70%;
    text-align: justify;
  }

  .role {
    font-size: 15px;
    color: white;
    background-color: var(--rhs-green);
    padding: 15px;
    margin-top: 15px;
    margin-right: 15px;
    list-style-type: none;
  }
</style>
