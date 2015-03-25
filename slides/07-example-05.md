## Town-Lines controller

- Una vez que tengamos los estados bien configurados, crearemos un nuevo *controller*: *js/controllers/townLines.js*.

```
angular.module('townLines.controller', [])

.controller('TownLinesCtrl', function($scope, $stateParams, $http) {

    $http.get('http://openbizkaibus.appspot.com/api/LineasMunicipio?codmunicipio=' + $stateParams.townId)
        .then(function(resp) {

            $scope.linesInTown = resp.data;

        }, function(err) {

            console.error('ERR', err);

        })
})

```
- En este caso, además del *$http* necesitaremos el servicio **$stateParams**, para poder acceder a la variable de la URL.
