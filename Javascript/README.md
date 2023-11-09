# Sección JavaScript

## Hoisting

El concepto de Hoisting fue pensado como una manera general de referirse a cómo funcionan los contextos de ejecución en JavaScript (específicamente las fases de creación y ejecución).

## Variables

A la hora de crear variables en Javascript evitar usar VAR. En vez de eso usar let y const. Se caracterizan por tener un scope de bloque.

### const

Se utiliza cuandono se quiere que la variable cambie su valor, es decir que su valor es constante, no se puede cambiar su tipo de dato ni su valor. Algo muy interesante para los tipos de datos array y object pueden agregar mas elemento sin problemas.

```javascript
const name = "Nicolas";
const age = 25;
const isHuman = false;
const fruits = ["apple", "orange", "tomatp"];
const person = { name: "Juan", age: 30 };
```

### let

Se utiliza cuando se quiere que las variables cambien su valor y/o su tipo.

```javascript
let total = 0;
total = +20;
```

## template String

Permite habilitar el uso de expresiones de javascript incrustradas. Se pueden utilizar cadenas de caracteres de mas de una linea y funcionalidades de interpolacion de strings. Respet la posicion y los saltos de linea.

```javascript
let name = "Nicolas";
let age = 25;
let template = `Hola soy ${name} y tengo ${age}`;
```

## objetos literales

Toda variable en JavaScript tiene un prototype (un ADN basicamente), los objetos literales tambien son conocidos como diccionarios en otros lenguajes de programacion, suelen ser objetos con clave valor. los valores pueden ser cualquier tipo de datos de JavaScript.

```javascript
const person = {
  name: "Nicolas",
  lastname: "Perez",
  age: 20,
  getFullName: ()=> return `${name} ${lastname}`,
};

const person2 = person; // copia de la referencia el espacio en memoria
```
