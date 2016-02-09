### Enrutamiento
#### $routeParams

config()
```javascript
.when('/second/:num', {
    templateUrl: 'pages/second.html',
    controller: 'secondController'
})
```
controller()
```javascript
.controller('secondController', function($scope, $routeParams) {
    $scope.num = $routeParams.num;
})
```
second.html
```html
<h1>This is second!</h1>
<h3>Scope route value: {{num}}</h3>
```
