### Servicios
#### Factory II

```javascript
.controller('ListCtrl', function (taskList, $scope) {

    $scope.tasks = taskList.getList();

})

.controller('CreateCtrl', function (taskList, $scope) {

    $scope.newTask = '';
    
    $scope.addTask = function () {
        taskList.addTask($scope.newTask);
        $scope.newTask = '';
    }

})
```
