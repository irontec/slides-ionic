## Pestaña Towns

- Modificaremos el archivo *tab-towns.html* para mostrar los resultados que devuelve el *controller*.

```
<ion-view view-title="Municipios">
    <ion-content>
        <div ng-repeat="lineGroup in lineGroups">
            <div class="list">

                <div class="item item-divider">
                    {{lineGroup.DescripcionGrupo}}
                </div>

                <a class="item item-icon-right" ng-repeat="lines in lineGroup.Registros">
                    {{lines.DescripcionElemento}}
                    <i class="icon ion-ios-arrow-right"></i>
                </a>

            </div>
        </div>
    </ion-content>
</ion-view>
```
