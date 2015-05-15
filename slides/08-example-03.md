### Pestaña de información
#### Crear un *controller*


- Por cada pestaña, crearemos un *controller* dentro de la carpeta *js/controllers*.

- Empezaremos creando el archivo *about.js* con el siguiente contenido.

```
angular.module('about.controller', [])

.controller('aboutCtrl', function($scope) {
    $scope.Author = "Mikel Eizagirre";
    $scope.Description = "Ionic Framework - 2015";
});
```
