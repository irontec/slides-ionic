### Pestaña de información
#### Mostrar la lista de municipios

- Modificaremos el archivo *tab-towns.html* para mostrar los resultados que devuelve el *controller*.

```
<ion-view view-title="Municipios">
    <ion-content>
        <div ng-repeat="lineGroup in lineGroups">
            <ion-list>
                <ion-item class="item-divider">
                    {{lineGroup.DescripcionGrupo}}
                </ion-item>

                <ion-item class="item-icon-right" ng-repeat="lines in lineGroup.Registros">
                    {{lines.DescripcionElemento}}
                    <i class="icon ion-ios-arrow-right"></i>
                </ion-item>
            </ion-list>
        </div>
    </ion-content>
</ion-view>
```
