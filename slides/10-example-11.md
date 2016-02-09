### Pestañas anidadas
#### Mostrar la lista de líneas

- Crearemos un nuevo *template* en la carpeta *templates* con el nombre *tab-town-lines.html*.

```
<ion-view view-title="Líneas del municipio">
    <ion-content>
        <ion-list>
            <ion-item class="item-icon-right" ng-repeat="lineInTown in linesInTown">
                <span class="badge badge-positive">{{lineInTown.CodigoLinea}}</span>
                {{lineInTown.DenominacionLinea}}
            </ion-item>
        </ion-list>
    </ion-content>
</ion-view>
```
