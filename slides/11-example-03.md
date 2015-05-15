### Pestaña de una línea
#### Añadir un nuevo estado

```
$stateProvider.state('tab.lines', {
    url: '/lines/:lineId',
    views: {
        'tab-towns': {
            templateUrl: 'templates/tab-lines.html',
            controller: 'linesCtrl'
        }
    }
})
```
