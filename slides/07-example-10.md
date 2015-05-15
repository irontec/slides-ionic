### Rutas y estados
#### app.js

```javascript
.config(function($stateProvider, $urlRouterProvider) {
    $stateProvider.state('towns', {
        url: '/towns',
        views: {
            'towns': {
                templateUrl: 'templates/tab-towns.html',
            }
        }
    })

    $stateProvider.state('about', {
        url: '/about',
        views: {
            'about': {
                templateUrl: 'templates/tab-about.html',
            }
        }
    });

    $urlRouterProvider.otherwise('/towns');
});
```
