### Añadir info de una línea I

- Creamos un nuevo estado.

```
$stateProvider.state('tab.lines', {
    url: '/lines/:lineId',
    views: {
        'tab-towns': {
            templateUrl: 'templates/tab-lines.html',
            controller: 'lineCtrl'
        }
    }
})
```

- Creamos un *service* para esa pestaña.

```
angular.module('lines.service', [])

.factory('linesFactory', function($http, ApiEndpoint) {
	return {
		getLineInfo: function(lineId){
            return $http.get(ApiEndpoint.url + '/Buscar_TextoHorarioLinea?codlinea=' + lineId);
		}
	}
});
```
