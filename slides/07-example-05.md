### Añadir pestañas
#### Directivas utilizadas

- **```<ion-nav-bar>:```** Es la barra de navegación donde se mostrará el título de nuestra vista. Sustituirá el *header*.

- **```<ion-nav-view>:```** Es la directiva encargada de renderizar los templates del estado actual.

- **```<ion-tabs>:```** Es la directiva que se encargará de agrupar las pestañas.

- **```<ion-tab>:```** Si dicha pestaña está activa, creará un *content* según su contenido y gestionará su propio histórico.

- **```<ion-nav-view name="nombre">:```** Al haber más de una directiva al mismo nivel y cada uno existe en su propia pestaña, hay que darles un nombre para evitar conflictos en el *router*.
