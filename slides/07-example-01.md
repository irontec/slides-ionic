## Estados abstractos

- Añadiremos un nuevo estado abstracto para encapsular todas las pestañas y reutilizar código.

```
.state('tab', {
    url: "/tab",
    abstract: true,
    templateUrl: "templates/tabs.html"
})
```
- Como todas las pestañas tendrá la misma navegación, guardaremos el ```<ion-tabs>``` en el fichero *tabs.html*.

```
<ion-tabs class="tabs-icon-top tabs-positive">
  <ion-tab href="#/tab/towns" title="Municipios" icon-off="ion-ios-location-outline" icon-on="ion-ios-location">
    <ion-nav-view name="tab-towns"></ion-nav-view>
  </ion-tab>

  <ion-tab href="#/tab/about" title="Información" icon-off="ion-ios-information-outline" icon-on="ion-ios-information">
    <ion-nav-view name="tab-about"></ion-nav-view>
  </ion-tab>
</ion-tabs>
```
