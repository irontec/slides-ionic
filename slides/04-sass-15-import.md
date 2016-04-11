### Sass
#### @import

- Permite importar código de otro archivo.

```css
/* _reset.scss */

html,
body,
ul,
ol {
    margin: 0;
    padding: 0;
}
```

```css
/* base.scss */

@import 'reset';

body {
    font: 100% Helvetica, sans-serif;
    background-color: #efefef;
}
```
