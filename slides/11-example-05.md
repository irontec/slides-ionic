### Pestaña de una línea
#### Crear un nuevo *controller*

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
