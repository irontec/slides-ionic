### AngularJS
#### Inyección de dependencias I

- En vez de crear un objeto dentro de una función, pasarle el objeto a la función.

```javascript
var Person = function(firstname, lastname) {
    this.firstname = firstname;
    this.lastname = lastname;
}

function logPerson() {
    var john = new Person('John', 'Doe');
    console.log(john);
}

logPerson();
```
