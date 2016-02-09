### Servicios
#### Factory I

```javascript
.factory("taskList", function() {
    
    var tasks = [];

    var taskList = {
        getList: function(){
            return tasks;
        },
        addTask: function(task){
            tasks.push(task);
        }
    }

    return taskList;

})
```
