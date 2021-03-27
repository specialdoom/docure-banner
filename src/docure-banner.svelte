<svelte:options tag="docure-banner" />

<script>
  export let imagesrc = "";
  export let background = "";
</script>

<div
  class="docure-banner-image"
  style={`background-image: url(${imagesrc});`}
/>
<div class="docure-banner-body" style={`background: ${background};`}>
  <slot name="title" />
  <slot name="description" />
  <slot name="actions" />
</div>

<style>
  :host {
    display: flex;
    width: 100%;
    height: 400px;
  }

  .docure-banner-image {
    background-repeat: no-repeat;
    height: 100%;
    width: 800px;
  }

  .docure-banner-body {
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 40px 60px;
    width: calc(100vw - 800px);
    height: 100%;
  }

  slot[name="title"] {
    font-size: 24px;
    text-align: center;
    height: 30%;
  }

  slot[name="description"] {
    display: flex;
    height: 40%;
  }

  slot[name="actions"] {
    display: flex;
    align-items: center;
    height: 30%;
  }
</style>
