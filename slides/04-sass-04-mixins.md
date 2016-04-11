### Sass
#### @mixins

- Es posible declarar funciones para generar estilos en base a variables.

```css
@mixin border-radius($radius) {
    -webkit-border-radius: $radius;
       -moz-border-radius: $radius;
        -ms-border-radius: $radius;
            border-radius: $radius;
}

.box { @include border-radius(10px); }
```

<pre class="fragment">
    <code>.box {
    -webkit-border-radius: 10px;
    -moz-border-radius: 10px;
    -ms-border-radius: 10px;
    border-radius: 10px;
}</code>
</pre>
