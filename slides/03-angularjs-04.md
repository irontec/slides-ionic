### AngularJS
#### Renderizado en la parte del cliente

- El servidor proporciona los contenidos estáticos (**plantillas**) y la información que se va a mostrar (**modelo**).
- Es el cliente el encargado de mezclar dichos datos y generar la vista que se va a mostrar.

```
<div ng-app="miApp">
    <ul ng-controller="miControlador">
        <li ng-repeat="contacto in contactos">
            {{contacto.nombre}} ({{contacto.telefono}})
        </li>
    </ul>
</div>
```
