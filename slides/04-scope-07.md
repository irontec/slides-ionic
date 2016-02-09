### $scope
#### Nuestro primer controlador V

```javascript
angular.module('miApp', [])
    .controller('mainCtrl', function($scope) {
        $scope.name = '';

        console.log($scope);
    });
```

```html
<h1>¡Hola {{name}}!</h1>
<input type="text" ng-model="name">

```
