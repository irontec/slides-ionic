## Añadir Tabs

- En este punto vamos a cambiar los botones por pestañas.

- Para ello, eliminaremos el *footer* que hemos añadido y sustituiremos *```<ion-header-bar></ion-header-bar>```* con el siguiente código:

```
<ion-nav-bar class="bar-positive" title="BizkaiBus App">
</ion-nav-bar>
```

- También sustituiremos *```<ion-content></ion-content>```* por el siguiente código:

```
<ion-tabs class="tabs-icon-top tabs-positive">
  <ion-tab href="towns" title="Municipios" icon-off="ion-ios-location-outline" icon-on="ion-ios-location">
    <ion-nav-view name="towns"></ion-nav-view>
  </ion-tab>

  <ion-tab href="about" title="Información" icon-off="ion-ios-information-outline" icon-on="ion-ios-information">
    <ion-nav-view name="about"></ion-nav-view>
  </ion-tab>
</ion-tabs>
```
