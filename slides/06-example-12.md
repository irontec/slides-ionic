### Pestaña *About* II

- Para poder utilizar los valores de *Author* y *Description* del controller, deberemos inyectar el *about.controller* en *app.js*.

```
angular.module('starter', ['ionic', 'about.controller'])
```

- Por último, tenemos que incluir el about.js. Para ello en el index hay que añadir lo siguiente.

```
<script src="js/controllers/about.js"></ script>
```
