### Pestañas anidadas
#### Adaptar los estados II

- Y actualizaremos el **$urlRouterProvider** para que cargue bien la pestaña *towns*.

```
$urlRouterProvider.otherwise('/tab/towns');
```
- Para declarar que un estado es hijo de otro, se utiliza la notación '.': **padre.hijo** y lo mismo pasa con las URL: **padre/hijo**
