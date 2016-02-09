### Servicios
#### Constant

```javascript
angular.module('constantExample', [])
    .constant("myConfig", {
        "url": "http://localhost",
        "port": "80"
    })
    .controller('MainCtrl', function (myConfig, $scope) {
        $scope.config = myConfig;
    });
```
