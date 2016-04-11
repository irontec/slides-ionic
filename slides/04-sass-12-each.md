### Sass
#### Directivas de control y expresiones - @each

```css
@each $animal in puma, sea-slug, egret, salamander {
    .#{$animal}-icon {
        background-image: url('/images/#{$animal}.png');
    }
}
```

<pre class="fragment">
    <code>.puma-icon {
    background-image: url('/images/puma.png'); }
.sea-slug-icon {
    background-image: url('/images/sea-slug.png'); }
.egret-icon {
    background-image: url('/images/egret.png'); }
.salamander-icon {
    background-image: url('/images/salamander.png'); }</code>
</pre>
