### Pestañas anidadas
#### Crear un nuevo servicio

- A continuación crearemos el servicio *js/services/townLines.js*

```
angular.module('townLines.service', [])

.factory('townLinesFactory', function($http, ApiEndpoint) {
	return {
		getTownLines: function(townId){
            return $http.get(ApiEndpoint.url + '/LineasMunicipio?codmunicipio=' + townId);
		}
	}
});

```
