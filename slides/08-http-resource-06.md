### $http
#### Promesas


- Para gestionar los posibles eventos de **éxito o fracaso de la petición**, tenemos que contemplar los dos casos:

```
$http.get("http://example.com/url/ajax")
.then(function(res){
    // acciones a realizar cuando se recibe respuesta con éxito
}, function(res){
    // acciones a realizar cuando se recibe una respuesta de error
});
```
