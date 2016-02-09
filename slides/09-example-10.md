### Solucionar el error CORS III

- Actualizaremos el *townsFactory* para utilizar la constante que acabamos de definir.

```
angular.module('town.service', [])

.factory('townsFactory', function($http, ApiEndpoint) {
	return {
		getTowns: function(){
            return $http.get(ApiEndpoint.url + '/Consultar_FamiliasCentros');
		}
	}
});

```
