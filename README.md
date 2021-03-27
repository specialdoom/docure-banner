### docure-banner

```js
npm i @specialdoom/docure-banner
```

### usage

```html
<docure-banner imagesrc="https://www.cflowapps.com/wp-content/uploads/2018/06/workflow-optimization.png"
    background="#e5e9ff">
    <p slot="title">Nec dui nunc</p>
    <div slot="description">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
      tempor incididunt ut labore et dolore magna aliqua. Faucibus ornare
      suspendisse sed nisi lacus. Justo eget magna fermentum iaculis eu.
    </div>
    <span slot="actions">
      <a href='something'>Something</a>
      <a href='something-else'>Something else </a>
    </span>
</docure-banner>
```

### attributes
- _imagesrc_ source for banner image
- _background_ background for banner text

### slots
- _slot="title"_ for banner titles
- _slot="description"_ for banner description
- _slot="actions"_ for banner actions

The slot attribute can be added on any element.

### example 

![Presentation](presentation.png)