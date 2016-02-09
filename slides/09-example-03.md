### Pestaña de información
#### Servicio para conseguir la lista de municipios

- Crearemos un servicio en la carpeta *js/services* con el nombre towns.js.

```
angular.module('town.service', [])

.factory('townsFactory', function($http) {
	return {
		getTowns: function(){
            return $http.get('http://openbizkaibus.appspot.com/api/Consultar_FamiliasCentros');
		}
	}
});
```

- Necesitaremos el servicio *$http* para hacer consultas.
