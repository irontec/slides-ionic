## Añadir info de una línea I

- Creamos un nuevo estado.

```
$stateProvider.state('tab.lines', {
    url: '/lines/:lineId',
    views: {
        'tab-towns': {
            templateUrl: 'templates/tab-lines.html',
            controller: 'LineCtrl'
        }
    }
})
```

- Creamos un *controller* para esa pestaña.

```
angular.module('lines.controller', [])

.controller('LinesCtrl', function($scope, $stateParams, $http) {

    $http.get('http://openbizkaibus.appspot.com/api/Buscar_TextoHorarioLinea?codlinea=' + $stateParams.lineId)
        .then(function(response) {

            $scope.line = response.data;

        }, function(err) {

            console.error('ERR', err);

        })
})
```
