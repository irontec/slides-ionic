### Enlaces externos

- Para añadir enlaces externos, hay que instalar el plugin Cordova InAppBrowser.

```
cordova plugin add https://git-wip-us.apache.org/repos/asf/cordova-plugin-inappbrowser.git
```

- Añadimos el siguiente código en index.html, para interceptar enlaces externos y consumir el touch.

```
<script>
document.addEventListener('click', function (e) {
    e = e ||  window.event;
    var element = e.target || e.srcElement;
    if (element.tagName == 'A') {
        if (element.href.length > 0 && element.href.indexOf('#') === -1 ) {
            window.open(element.href, "_system", "location=yes");
            e.preventDefault();
        }
    }
}, true);
</ script>
```
