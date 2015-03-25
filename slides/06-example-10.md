## Pestaña *About*

- Para terminar, personalizaremos la pestaña *about* con elementos *card*, *item*, *avatar*...

```
<ion-view view-title="Información">
    <ion-content>
        <div class="list card">
            <div class="item item-avatar">
                <img src="img/author.png">
                <h2>{{Author}}</h2>
                <p>{{Description}}</p>
            </div>
            <div class="item item-image">
                <img src="img/ironlogo.jpeg">
            </div>
        </div>
    </ion-content>
</ion-view>
```

- Para poder utilizar los valores de *Author* y *Description* del controller, deberemos inyectar el *about.controller* en *app.js*.

```
angular.module('starter', ['ionic', 'about.controller'])
```
