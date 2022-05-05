<script lang="ts">
  import Cards from "./Cards.svelte";
  import Push from "./Push.svelte";

  export let name: string;
</script>

<main>
  <Cards />
  <Push namee={name} />
</main>

<style lang="scss">
  @import "./styles/vars";
  @import "./styles/classes";

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
