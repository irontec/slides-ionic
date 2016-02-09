### Enrutamiento
#### Configurar el $routeProvider I

- Nos permite **configurar las rutas** que queremos crear de una manera declarativa.

- $routeprovider tiene dos métodos:
    - **when():** nos sirve para indicar qué se debe hacer en cada ruta.
    - **otherwise():** para marcar un comportamiento cuando se intente acceder a cualquier otra ruta no declarada.

- Esta configuración se debe realizar dentro del **método config()**.

```javascript
angular.module("app", ["ngRoute"])
    .config(function($routeProvider){
	//configuración y definición de las rutas
    });
```
