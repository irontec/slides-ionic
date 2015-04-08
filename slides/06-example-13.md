## Towns Controller II

- Modificaremos de nuevo el *app.js*, para añadir el *controller TownsCtrl* al estado *towns*.

```
$stateProvider.state('towns', {
    url: '/towns',
    views: {
        towns: {
            templateUrl: 'templates/tab-towns.html',
            controller: 'TownsCtrl'
        }
    }
})
```

- También habrá que especificar la inyección de dependencias en *angular.module* e incluir el *towns.js*

```
angular.module('starter', ['ionic', 'about.controller', 'town.controller'])
```

```
<script src="js/controllers/towns.js"></ script>
```
