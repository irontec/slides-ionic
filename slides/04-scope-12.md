### $scope
#### Jerarquías III

```javascript
angular.module('scopeExample', [])
    .controller('GreetController', function($scope, $rootScope) {
        $scope.name = 'World';
        $rootScope.department = 'Angular';
    })
    .controller('ListController', function($scope) {
        $scope.names = ['Igor', 'Misko', 'Vojta'];
    });
```
