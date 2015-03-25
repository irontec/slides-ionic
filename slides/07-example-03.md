## Adaptar los estados II

- Por último, haremos lo mismo con el estado *about*. Pasará a llamarse **tab.about**.

```
.state('tab.about', {
    url: '/about',
    views: {
        'tab-about': {
            templateUrl: 'templates/tab-about.html',
            controller: 'AboutCtrl'
        }
    }
});
```
- Y actualizaremos el **$urlRouterProvider** para que cargue bien la pestaña *towns*.

```
$urlRouterProvider.otherwise('/tab/towns');
```
