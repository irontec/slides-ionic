### Pestaña de información
#### *Controller* para gestionar la pestaña

- Crearemos otro controller en la carpeta *js/controllers* con el nombre towns.js.

```
angular.module('town.controller', [])

.controller('townsCtrl', function($scope, townsFactory) {

    townsFactory.getTowns()
        .then(function(towns) {

            $scope.lineGroups = towns.data;

        }, function(err) {

            console.error('ERR', err);

        })
})
```
