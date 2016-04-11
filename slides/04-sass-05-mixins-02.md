### Sass
#### @mixins II

```css
.box-10 { @include border-radius(10px); }
.box-rect { @include border-radius(0px); }
```

<pre class="fragment">
    <code>.box-10 {
    -webkit-border-radius: 10px;
       -moz-border-radius: 10px;
        -ms-border-radius: 10px;
            border-radius: 10px;
}

.box-rect {
    -webkit-border-radius: 0px;
       -moz-border-radius: 0px;
        -ms-border-radius: 0px;
            border-radius: 0px;
}</code>
</pre>
