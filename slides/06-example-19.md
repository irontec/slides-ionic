## Solucionar el error CORS IV

- Para automatizar la tarea de añadir/quitar el *proxy* utilizaremos *Gulp*.

- Primero instalaremos el módulo ```replace```.

```
npm install --save replace
```

- A continuación añadiremos las tareas ```add-proxy``` y ```remove-proxy```.

```
var replace = require('replace');
var replaceFiles = ['./www/js/app.js'];
```
```
gulp.task('add-proxy', function() {
  return replace({
    regex: "http://openbizkaibus.appspot.com/api",
    replacement: "http://localhost:8100/api",
    paths: replaceFiles,
    recursive: false,
    silent: false,
  });
})
```
```
gulp.task('remove-proxy', function() {
  return replace({
    regex: "http://localhost:8100/api",
    replacement: "http://openbizkaibus.appspot.com/api",
    paths: replaceFiles,
    recursive: false,
    silent: false,
  });
})
```
