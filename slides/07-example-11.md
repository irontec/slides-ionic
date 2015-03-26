## Añadir info de una línea II

- Creamos un nuevo *template*.

```
<ion-view view-title="Información de la línea">
  <ion-content>
    <div class="card">
      <div class="item item-text-wrap">
        <p ng-bind-html="line.TextoVuelta"></p>
      </div>
    </div>
    <div class="card">
      <div class="item item-text-wrap">
        <p ng-bind-html="line.TextoIda"></p>
      </div>
    </div>
  </ion-content>
</ion-view>
```

- Inyectamos el *controller* en el módulo general de *app.js*, incluimos el *.js* y añadimos el cambio de estado en el *template* *tab-town-lines.html*.

```
angular.module('starter', ['ionic', ..., 'lines.controller'])
```

```
<script src="js/controllers/lines.js"></ script>
```
```
<a ng-repeat="lineInTown in linesInTown" href="#/tab/lines/{{lineInTown.CodigoLinea}}">
```
