# Templates

Use the photon-ref tag to use a template.

The src attribute of the photon-ref element specifies the path to the template file. Data-attributes are used to fill the placeholders in the template.

<br />

Example:

Inside /src/index.html

```html
<photon-ref
  src="./templates/anchor.html"
  data-href="https://github.com/photon-framework"
  data-content="source"
></photon-ref>
```

/src/templates/anchor.html

```html
<a
  target="_blank"
  href="{{href}}"
  rel="noopener noreferrer"
  title="{{href}}"
  class="{{class}}"
  >{{content}}</a
>
```
