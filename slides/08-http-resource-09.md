### $http
#### Alertar si algo ha ido mal


- Para gestionar los posibles eventos de **éxito o fracaso de la petición**, tenemos que contemplar los dos casos:

```
$http.get("http://restcountries.eu/rest/v1/region/europe")
    .then(function(res){
        console.log(res);
        $scope.countries = res.data;
    }, function(res){
        console.log(res);
        $window.alert('Error')
    });
```
