### Pestañas anidadas
#### Añadir un nuevo estado

- Una vez que tengamos los estados bien configurados, añadiremos un nuevo estado *town-lines*.

```
$stateProvider.state('tab.town-lines', {
    url: '/towns/:townId',
    views: {
        'tab-towns': {
            templateUrl: 'templates/tab-town-lines.html',
            controller: 'townLinesCtrl'
        }
    }
})
```
