## Towns Controller I

- Crearemos otro controller en la carpeta *js/controllers* con el nombre towns.js.

```
angular.module('town.controller', [])

.controller('TownsCtrl', function($scope, $http) {

    $http.get('http://openbizkaibus.appspot.com/api/Consultar_FamiliasCentros')
        .then(function(resp) {

            $scope.lineGroups = resp.data;

        }, function(err) {

            console.error('ERR', err);

        })
});
```

- En este caso, necesitaremos el servicio *$http* para hacer consultas al [API de BizkaiBus](http://openbizkaibus.appspot.com/api/).
