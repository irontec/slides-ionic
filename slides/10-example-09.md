### Pestañas anidadas
#### Crear un nuevo *controller*

- También crearemos un nuevo *controller*: *js/controllers/townLines.js*.

```
angular.module('townLines.controller', [])

.controller('townLinesCtrl', function($scope, $stateParams, townLinesFactory) {

    townLinesFactory.getTownLines($stateParams.townId)
        .then(function(townLines) {

            $scope.linesInTown = townLines.data;

        }, function(err) {

            console.error('ERR', err);

        })
})

```
- En este caso, necesitaremos el servicio **$stateParams**, para poder acceder a la variable de la URL.
