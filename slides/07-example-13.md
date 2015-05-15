### Añadir info de una línea III

- Creamos un nuevo *template*.

```
<ion-view view-title="Información de la línea">
  <ion-content>
    <div class="card">
      <div class="item item-text-wrap">
        <p ng-bind-html="line.TextoVuelta"></p>
      </div>
    </div>
    <div class="card">
      <div class="item item-text-wrap">
        <p ng-bind-html="line.TextoIda"></p>
      </div>
    </div>
  </ion-content>
</ion-view>
```
