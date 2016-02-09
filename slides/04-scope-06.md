### $scope
#### Nuestro primer controlador IV

```javascript
angular.module('miApp', [])
    .controller('mainCtrl', function($scope) {
        $scope.name = 'Mikel';

        $scope.getName = function() {
            return $scope.name;
        }

        console.log($scope);
    });
```

```html
<h1>¡Hola {{getName()}}!</h1>
```
