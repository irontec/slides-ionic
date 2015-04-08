## Solucionar el error CORS I

- Para solucionar ese error, hay que hacer peticiones al servidor sin especificar el ```origin```.

- Para resolver este tipo de errores, el *CLI* de ionic proporciona la opción de utilizar servidores *proxy*.

- Para ello, modificaremos el archivo *ionic.project*.

```
"proxies": [
    {
      "path": "/api",
      "proxyUrl": "http://openbizkaibus.appspot.com/api"
    }
  ]
```
