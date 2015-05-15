### Sass
#### Anidar selectores

- Permite anidar selectores para estructurar mejor el código.

```css
nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li { display: inline-block; }

  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```

- El código anterior, afectaría solamente a los ```ul```, ```li``` y ```a``` que se encuentran dentro de ```nav```.
