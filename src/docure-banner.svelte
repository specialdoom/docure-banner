<svelte:options tag="docure-banner" />

<script>
  export let imagesrc = '';
</script>

<div class="docure-banner-content"><slot /></div>
<div
  class="docure-banner-image"
  style={`background-image: url(${imagesrc}); background-size: auto 400px; background-repeat: no-repeat`}
/>

<style>
  :host {
    display: flex;
    position: relative;
    width: 100%;
    height: 400px;
  }

  :host div.docure-banner-content {
    width: 70%;
    height: 100%;
    display: flex;
    flex-direction: column;
    box-sizing: border-box;
    background: #dc493a;
    padding: 10px 30px;
  }

  :host div.docure-banner-image {
    width: 30%;
  }

  div.docure-banner-image::before {
    position: absolute;
    display: block;
    content: ' ';
    top: 0;
    bottom: 0;
    right: 0;
    left: 70%;
    background-image: url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxNjUuOCAyMDIiPjxkZWZzPjxzdHlsZT4uY2xzLTF7ZmlsbDojZGM0OTNhO30uY2xzLTJ7ZmlsbDojZmZmO308L3N0eWxlPjwvZGVmcz48ZyBpZD0iTGF5ZXJfMiIgZGF0YS1uYW1lPSJMYXllciAyIj48ZyBpZD0iTGF5ZXJfMS0yIiBkYXRhLW5hbWU9IkxheWVyIDEiPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTAsMFM3My43LDcuOCw3MS4yLDQzYy0uOCwxMS40LTYuNCwyNC41LS4zLDMzLjMsNy4zLDEwLjMsMjQuNSwzLjksMzAsMTUuN3MtOC4zLDI2LjktMy42LDM5LjRjMi44LDcuNSwxMS4yLDkuNiwxOCw3LjlzMTMuMS01LjksMjAtNy4xYzkuOS0xLjYsMjAuNCw0LDI2LDEzLjlzNiwyMy44LDEuMSwzNC4yLTE0LDE2LjUtMjMuNCwxOS4zLTI5LjEsMi4yLTI5LjEsMi4yTDU1LDIwMkgwIi8+PHBhdGggY2xhc3M9ImNscy0yIiBkPSJNMzQsMTk3LjRhNS43LDUuNywwLDAsMS0xLjgtLjN2LS41YTUuOCw1LjgsMCwwLDAsNS4yLS44YzIuNy0xLjksNS4xLTUuNyw2LTkuOS40LTIuMS42LTQuMy45LTYuNC41LTQuMiwxLTguNSwyLjktMTIuMXM3LjQtOCwxNC44LTkuOWw0LjQtLjljNC4yLS45LDguNS0xLjgsMTIuNC00czkuMy05LjIsOC4xLTE1LjdjLTEuNi04LjItMTAuNS0xMS4zLTE4LjctMTAuN2wtMy45LjNjLTYuNi42LTEzLjQsMS4yLTE4LjctMy03LjctNi4xLTcuNy0xOC42LTcuMS0yNS42LjItMi4xLjUtNC4zLjgtNi40LjktNy4xLDEuOC0xNC40LjEtMjEuMlMzMS42LDU1LjYsMjQuNiw1My40QTIwLjEsMjAuMSwwLDAsMCw0LjEsNTguOWwtLjMtLjNhMjAuNSwyMC41LDAsMCwxLDIwLjktNS43YzcuMiwyLjMsMTMuMSw5LjEsMTUuMiwxNy4zcy44LDE0LjItLjEsMjEuM2MtLjMsMi4yLS42LDQuMy0uOCw2LjUtLjYsNi44LS42LDE5LjIsNi45LDI1LjEsNS4yLDQuMiwxMiwzLjUsMTguNSwyLjlsMy45LS4zYzguMy0uNSwxNy40LDIuNywxOS4xLDExLjEsMS4zLDYuNy0zLjIsMTMuMi04LjQsMTYuMnMtOC4yLDMuMS0xMi40LDRsLTQuNCwxYy03LjMsMS44LTEyLDQuOS0xNC42LDkuNnMtMi4zLDcuOC0yLjgsMTJjLS4zLDIuMS0uNSw0LjMtMSw2LjQtLjksNC4zLTMuMyw4LjMtNi4xLDEwLjJBNi44LDYuOCwwLDAsMSwzNCwxOTcuNFoiLz48L2c+PC9nPjwvc3ZnPg==');
    background-size: auto 400px;
    background-repeat: no-repeat;
  }
</style>
