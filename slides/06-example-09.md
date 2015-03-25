## *Controllers*


- Por cada pestaña, crearemos un *controller* dentro de la carpeta *js/controllers*.

- Empezaremos creando el archivo *about.js* con el siguiente contenido

```
angular.module('about.controller', [])

.controller('AboutCtrl', function($scope) {

    $scope.Author = "Mikel Eizagirre";
    $scope.Description = "Ionic Framework - 2015";

});
```
- Además, debemos modificar el estado *about* para que cargue el controller *AboutCtrl*.

```
$stateProvider.state('about', {
    url: '/about',
    views: {
        about: {
            templateUrl: 'templates/tab-about.html',
            controller: 'AboutCtrl'
        }
    }
});
```
