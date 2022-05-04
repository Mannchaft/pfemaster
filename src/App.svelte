<script lang="ts">
  export let name: string;
  let a: Boolean;
  a = false;
  function click() {
    if (!a) {
      name = "Worldi";
    } else {
      name = "World";
    }
    a = !a;
  }
</script>

<main>
  <h1>Hello {name}!</h1>
  <button class="button-29" on:click={click}>Slight change</button>
</main>

<style type="text/scss">
  @import "./styles/vars";
  @import "./styles/classes";

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
