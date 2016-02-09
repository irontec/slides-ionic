### Directivas
#### ngClass

- Nos permite especificar clases de **CSS dinámicamente**.
- Formas de uso:
    - Si la expresión a evaluar es un **string**, será una **lista de nombres de clase** separado por espacios.
    - Si la expresión a evaluar es un **objeto**, por cada **clave-valor** si el valor es true se añadira la clase clave.
    - Si la expresión a evaluar es un **array**, cada elemento será un string del tipo 1 o un objeto del tipo 2.

- Las clases **no se duplican**.
- Si la expresión cambia **se recalculan** los estilos.
