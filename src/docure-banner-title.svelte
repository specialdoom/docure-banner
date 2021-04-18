<svelte:options tag="docure-banner-title" />

<script>
  export let text = '';
</script>

<p>
  {text}
</p>

<style>
  :host {
    height: 20%;
  }
  :host p {
    color: white;
    text-align: left;
    font-size: large;
    font-weight: bold;
    text-transform: uppercase;
  }
</style>
