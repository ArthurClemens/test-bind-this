<script>
  // DOM binding
  let domElement;

  export let label;

  const onClick = e => {
    e.preventDefault();
    console.log("onClick", e);
    console.log("domElement=", domElement);
  };

</script>

<style>
.button {
  padding: 6px 12px;
  border: 1px solid currentColor;
  display: inline-block;
  border-radius: 3px;
}
.button:hover {
  text-decoration: none;
}
</style>

<a class="button" bind:this={domElement} on:click={onClick} href="/">{label} - domElement={domElement}</a>
