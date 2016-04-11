### Sass
#### Directivas de control y expresiones - @for

```css
@for $i from 1 through 3 {
    .item-#{$i} { width: 2em * $i; }
}
```

<pre class="fragment">
    <code>.item-1 {
    width: 2em; }
.item-2 {
    width: 4em; }
.item-3 {
    width: 6em; }</code>
</pre>
