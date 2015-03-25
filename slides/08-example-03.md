## Eliminar contenido innecesario

- Para ocultar las secciones vacías, hay que añadir la directiva **ng-show** al elemento *item-divider*.

```
<div class="item item-divider" ng-show="(lineGroup.Registros | filter:search.value).length">
    {{lineGroup.DescripcionGrupo}}
</div>
```
