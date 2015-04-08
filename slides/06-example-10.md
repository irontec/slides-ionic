## Pestaña *About*

- Personalizaremos la pestaña *about* utilizando el siguiente código.

```
<ion-view view-title="Información">
    <ion-content>
        <div class="list card">
            <div class="item item-avatar">
                <img src="https://avatars0.githubusercontent.com/u/1042187?v=3&s=460">
                <h2>{{Author}}</h2>
                <p>{{Description}}</p>
            </div>
            <div class="item item-image">
                <img src="https://pbs.twimg.com/profile_images/512504893165158400/dJv2Rrk4.jpeg">
            </div>
        </div>
    </ion-content>
</ion-view>
```

- Para poder utilizar los valores de *Author* y *Description* del controller, deberemos inyectar el *about.controller* en *app.js*.

```
angular.module('starter', ['ionic', 'about.controller'])
```

- Por último, tenemos que incluir el about.js. Para ello en el index hay que añadir lo siguiente.

```
<script src="js/controllers/about.js"></ script>
```
