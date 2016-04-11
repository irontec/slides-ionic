### Sass
#### Directivas de control y expresiones - @each II

```css
@each $header, $size in (h1: 2em, h2: 1.5em, h3: 1.2em) {
    #{$header} {
        font-size: $size;
    }
}
```

<pre class="fragment">
    <code>h1 {
    font-size: 2em; }
h2 {
    font-size: 1.5em; }
h3 {
    font-size: 1.2em; }</code>
</pre>
