## Solucionar el error CORS III

- Actualizaremos el *TownsCtrl* para utilizar la constante que acabamos de definir.

```
.controller('TownsCtrl', function($scope, $http, ApiEndpoint) {

    $http.get(ApiEndpoint.url + '/Consultar_FamiliasCentros')
        .then(function(resp) {

            $scope.lineGroups = resp.data;

        }, function(err) {

            console.error('ERR', err);

        })

})
```
