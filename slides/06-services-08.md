### Servicios
#### Factory IV

html
```html
<ul ng-controller="ListCtrl">
    <li ng-repeat="task in tasks">
    {{task.name}}
    <span class="glyphicon glyphicon-remove" ng-click="removeTask(task)"></span>
    </li>
</ul>
```
controller()
```javascript
$scope.removeTask = function(task) {
    console.log('remove task!');
    task.removed = true;
}
```
factory()
```javascript
addTask: function(task){
    tasks.push({name:task, removed: false});
}
```
