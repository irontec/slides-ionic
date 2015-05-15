### Buscador de municipios

- Para añadir un pequeño buscador, en el archivo *tab-towns.html* añadiremos el siguiente código.

```
<div class="bar item-input-inset">
    <label class="item-input-wrapper">
        <i class="icon ion-ios-search placeholder-icon"></i>
        <input type="search" placeholder="Buscar..." ng-model="search.value">
    </label>
    <button class="button button-clear" ng-click="search.value=''">
        Cancelar
    </button>
</div>
```

- Una vez que tengamos el buscador con el **ng-model** = *search.value*, lo único que falta es filtrar los datos.

```
ng-repeat="lines in lineGroup.Registros | filter:search.value"
```
