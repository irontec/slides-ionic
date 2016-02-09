### $http
#### Analizar la respuesta


- Para gestionar los posibles eventos de **éxito o fracaso de la petición**, tenemos que contemplar los dos casos:

```
$http.get("http://restcountries.eu/rest/v1/region/europe")
    .then(function(res){
        console.log(res);
    }, function(res){
        console.log(res);
    });
```
