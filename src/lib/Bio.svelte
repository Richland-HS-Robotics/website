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

<div id="small-container" on:click={() => (showModal = true)}>
  <img {src} />
  <div>
    <span class="name">{name}</span>
    <ol>
      {#each roles as role}
        <span class="role">{@html role}</span>
        <br />
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
    border-radius: 1.5em 1.5em;
    box-shadow: 5px 5px 5px #c7c7d1;
    cursor: pointer;
  }

  #small-container > img {
    height: 100%;
    border-radius: 0.5em 0.5em;
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
    border-radius: 0.7em 0.7em;
  }

  .p {
    width: 70%;
  }

  p {
    text-align: justify;
  }

  .role {
    font-size: 1.3em;
    background-color: #a2c5ac;
    padding: 0.2em;
    border-radius: 0.4em 0.4em;
    margin-left: 0.1em;
    margin-right: 0.1em;
    box-shadow: 3px 3px 3px #53a274;
  }
</style>
