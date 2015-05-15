### Añadir info de una línea II

- Creamos un *controller* para esa pestaña.

```
angular.module('lines.controller', [])

.controller('linesCtrl', function($scope, $stateParams, linesFactory) {

    linesFactory.getLineInfo($stateParams.lineId)
        .then(function(lineInfo) {
            $scope.line = lineInfo.data;

        }, function(err) {
            console.error('ERR', err);
        })
})
```
