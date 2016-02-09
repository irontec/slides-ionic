### Pestañas anidadas
#### Mejorar navegación

- Necesitaremos modificar el archivo *tab-towns.html* para añadir el **href** para el cambio de estado.

```
<a class="item item-icon-right" href="#/tab/towns/{{lines.CodigoElemento | numberFixedLen:3}}" ng-repeat="lines in lineGroup.Registros">
    {{lines.DescripcionElemento}}
    <i class="icon ion-ios-arrow-right"></i>
</a>

```

- Para asegurarnos de que el *townId* siempre tiene 3 dígitos:

```
.filter('numberFixedLen', function () {
  return function (n, len) {
      var num = parseInt(n, 10);
      len = parseInt(len, 10);
      if (isNaN(num) || isNaN(len)) {
          return n;
      }
      num = ''+num;
      while (num.length < len) {
          num = '0'+num;
      }
      return num;
  };
})
```
