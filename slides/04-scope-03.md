### $scope
#### Nuestro primer controlador I

```javascript
angular.module('miApp', [])
    .controller('mainCtrl', function() {
        console.log('Hola mundo!');
    });
```

```html
<body ng-app="miApp">
    <div ng-controller="mainCtrl">
    </div>
```
