### Pestañas anidadas
#### Diferencias entre tipos de estado

- **Estado abstracto:**
    - No se puede navegar a dicho estado.
    - Su objetivo es tener varios hijos con un padre común, sin tener que declarar un estado que pueda ser llamado.
    - Es activado implicitamente cada vez que un hijo suyo se activa.

- **Estados anidados:**
    - Son estados que pueden ser activados directamente.
    - La URL de estados hijos, es relativo a su padre. En este caso */tab/estadoActual*.
