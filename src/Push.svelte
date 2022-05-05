<script lang="ts">
  export let namee: string;
  let a: Boolean;
  a = false;
  function click() {
    if (!a) {
      namee = "Scripts";
    } else {
      namee = "Script";
    }
    a = !a;
  }
</script>

<h4>choose your {namee}!</h4>
<label for="script">Script:</label>

<textarea id="script" name="script" rows="15" cols="80">
  conf t enable secret islem username islem password islem line vty 0 4 login
  local transport input all end conf t int f0 no sh ip address dhcp end wr
</textarea>
<br />
<button class="button-29" on:click={click}>Slight change</button>

<style lang="scss">
  @import "./styles/vars";
  @import "./styles/classes";
</style>
