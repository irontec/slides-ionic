### Enrutamiento
#### Configurar el $routeProvider II

```javascript
.config(function($routeProvider){
    $routeProvider
        .when('/', {
            templateUrl: 'pages/main.html',
            controller: 'mainController'
        })
        .when('/second', {
            templateUrl: 'pages/second.html',
            controller: 'secondController'
        })
})

.controller('mainController', function() {})

.controller('secondController', function() {})
```
