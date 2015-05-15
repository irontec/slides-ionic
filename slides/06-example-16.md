### Towns Controller II

- Modificaremos de nuevo el *app.js*, para añadir el *controller townsCtrl* al estado *towns*.

```javascript
$stateProvider.state('towns', {
    url: '/towns',
    views: {
        towns: {
            templateUrl: 'templates/tab-towns.html',
            controller: 'townsCtrl'
        }
    }
})
```

- También habrá que especificar la inyección de dependencias en *angular.module* e incluir el *towns.js*

```javascript
angular.module('starter', ['ionic', 'about.controller', 'town.controller', 'town.service'])
```

```html
<script src="js/controllers/towns.js"></ script>
<script src="js/services/towns.js"></ script>
```
