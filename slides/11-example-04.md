### Pestaña de una línea
#### Crear un nuevo servicio


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
