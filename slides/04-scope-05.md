### $scope
#### Nuestro primer controlador III

```javascript
angular.module('miApp', [])
    .controller('mainCtrl', function($scope) {
        $scope.name = 'Mikel';
        console.log($scope);
    });
```

```html
<h1>¡Hola {{name}}!</h1>
```
