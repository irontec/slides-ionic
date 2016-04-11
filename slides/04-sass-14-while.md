### Sass
#### Directivas de control y expresiones - @while

- Permite importar código de otro archivo.

```css
$i: 6;
@while $i > 0 {
    .item-#{$i} { width: 2em * $i; }
    $i: $i - 2;
}
```

<pre class="fragment">
    <code>.item-6 {
    width: 12em; }

.item-4 {
    width: 8em; }

.item-2 {
    width: 4em; }</code>
</pre>
