## Solucionar el error CORS II

- Añadiremos la constante *ApiEndpoint* en el módulo general de la aplicación.

```
angular.module('starter', ['ionic', 'about.controller', 'town.controller'])
    .constant('ApiEndpoint', {
        url: 'http://localhost:8100/api'
    })
```
