### Pestaña de una línea
#### Inyectar dependencias e incluir js

- Inyectamos el *controller* en el módulo general de *app.js*, incluimos el *.js* y añadimos el cambio de estado en el *template* *tab-town-lines.html*.

```
angular.module('starter', ['ionic', ..., 'lines.controller', 'lines.service'])
```

```
<script src="js/controllers/lines.js"></ script>
<script src="js/services/lines.js"></ script>
```
```
<a ng-repeat="lineInTown in linesInTown" href="#/tab/lines/{{lineInTown.CodigoLinea}}">
```
