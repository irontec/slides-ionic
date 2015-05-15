### Pestañas anidadas
#### Añadir dependencias e incluir js

- Y de nuevo tenemos que inyectar dicho *controller* en el módulo general de *app.js* e incluir el *.js* en el *index.html*.

```
angular.module('starter', ['ionic', ..., 'townLines.controller', 'townLines.service'])
```

```
<script src="js/controllers/townLines.js"></ script>
<script src="js/services/townLines.js"></ script>
```
