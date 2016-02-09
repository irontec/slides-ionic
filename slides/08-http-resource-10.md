### $http
#### ngChange


- Para volver a hacer peticiones si una opción ha cambiado, se puede utilizar la directiva *ngChange*.

```javascript
$scope.reloadCountries = function() {
    $http.get($scope.url)
        .then(function(res){
            $scope.countries = res.data;
        }, function(res){
            $window.alert('Error')
        });
}
```
```html
<select ng-model="url" ng-change="reloadCountries()">
   <option value="http://restcountries.eu/rest/v1/region/africa">Africa</option>
    <option value="http://restcountries.eu/rest/v1/region/europe">Europa</option>
    <option value="http://restcountries.eu/rest/v1/region/americas">America</option>
 </select>
 ```
