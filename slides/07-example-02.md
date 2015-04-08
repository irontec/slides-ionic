## Adaptar los estados I

- Añadiremos el nuevo estado *TownLines* y modificaremos *Towns* para que sean hijos de *Tab*.

```
$stateProvider.state('tab.towns', {
    url: '/towns',
    views: {
        'tab-towns': {
            templateUrl: 'templates/tab-towns.html',
            controller: 'TownsCtrl'
        }
    }
})
$stateProvider.state('tab.town-lines', {
    url: '/towns/:townId',
    views: {
        'tab-towns': {
            templateUrl: 'templates/tab-town-lines.html',
            controller: 'TownLinesCtrl'
        }
    }
})
```

- Para declarar que un estado es hijo de otro, se utiliza la notación '.': **padre.hijo** y lo mismo pasa con las URL: **padre/hijo**
