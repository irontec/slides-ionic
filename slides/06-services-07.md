### Servicios
#### Factory III

```html
<body ng-app="constantExample">
  <div>
    <ul ng-controller="ListCtrl">
        <li ng-repeat="task in tasks">{{task}}</li>
    </ul>
    <div ng-controller="CreateCtrl">
        <input type="text" ng-model="newTask">
        <button type="button" ng-click="addTask()">Añadir</button>
    </div>
  </div>
</body>
```
