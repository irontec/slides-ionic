### $scope
#### Detección de cambios

- La detección de cambios se lleva a cabo mediante el **dirty-checking**.

- Cada vez que se ejecuta el $scope.$apply lanza el *digest cycle*.

- Se comparan todos los valores contra los últimos valores conocidos y si alguno es diferente, se ejecuta el *listener*.

![](assets/digest.png)
