### Pestañas anidadas
#### Adaptar los estados

- Modificaremos los estados *Towns* y *About* para que sean hijos de *Tab*.

```
$stateProvider.state('tab.towns', {
    url: '/towns',
    views: {
        'tab-towns': {
            templateUrl: 'templates/tab-towns.html',
            controller: 'townsCtrl'
        }
    }
})
$stateProvider.state('tab.about', {
    url: '/about',
    views: {
        'tab-about': {
            templateUrl: 'templates/tab-about.html',
            controller: 'aboutCtrl'
        }
    }
});
```
