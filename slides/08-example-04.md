### Pestaña de información
#### Añadir el *controller* al estado

- Además, debemos modificar el estado *about* para que cargue el controller *aboutCtrl*.

```
$stateProvider.state('about', {
    url: '/about',
    views: {
        about: {
            templateUrl: 'templates/tab-about.html',
            controller: 'aboutCtrl'
        }
    }
});
```
