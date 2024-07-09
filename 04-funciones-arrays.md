# Funciones

Las funciones son un conjunto de sentencias que realizan una tarea específica y pueden devolver un valor.

```javascript
function nombreFuncion(parametro1, parametro2, ...) {
    // Código de la función
    return valor; // No es obligatorio que devuelva un valor
}
```

Ejemplo:

```javascript
function suma(a, b) {
    return a + b;
}

let resultado = suma(2, 3);
console.log(resultado); // 5
```

## Argumentos

Los argumentos de una función son los valores que se pasan a la función al llamarla.

```javascript
function suma(a, b) {
    return a + b;
}

let resultado = suma(2, 3);
console.log(resultado); // 5
```
Los argumentos serían `2` y `3`.

### Valores por defecto

```javascript
function suma(a, b, c = 3) {
    return a + b + c;
}

var resultado = suma(2, 3, 4);
var resultado1 = suma(2, 3);

console.log(resultado); // 9
console.log(resultado1); // 8 (c toma el valor por defecto)
```

## Funciones recursivas

Una función recursiva es aquella que se llama a sí misma.

```javascript
function factorial(n) {
    if (n === 0) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}

let resultado = factorial(5);
console.log(resultado); // 120
```

## Funciones predefinidas

Son funciones que vienen predefinidas en JavaScript.

- `eval()`: Evalúa una cadena de texto como si fuera código JavaScript. Nos dice si es un código válido o no. Para Strings.
- `isFinite()`: Nos dice si un número es finito o no. Para números.
- `isNan()`: Nos dice si un valor es NaN o no. Para números.
- `parseInt()`: Convierte una cadena de texto a un número entero. Para Strings.
- `parseFloat()`: Convierte una cadena de texto a un número decimal. Para Strings.
- `Date()`: Nos permite trabajar con fechas y horas.
- `String()`: Nos permite trabajar con cadenas de texto. Por ejemplo, para la fecha de antes, ya que se usa con milisegundos y así la hacemos legible.
- `Number()`: Nos permite trabajar con números. 

# Arrays

Un array es un objeto que almacena una colección de elementos.

La longitud de un array es dinámica, es decir, puede cambiar en tiempo de ejecución.

Formas de declarar un array:

```javascript
let nombreArray = [1, 2, 3, 4, 5];
```
```javascript
let nombreArray = new Array(1, 2, 3, 4, 5);
```

Un array puede contener diferentes tipos de datos.

```javascript
let nombreArray = [1, 'hola', true, 4.5];
```

Redefinir un array:

```javascript
let nombreArray = [1, 2, 3, 4, 5];
// Redefinir el array
nombreArray = [6, 7, 8, 9, 10];
// Redefinir un elemento del array
nombreArray[0] = 11;
```

## Índices

Los índices de un array empiezan en 0.

```javascript
let nombreArray = [1, 2, 3, 4, 5];
console.log(nombreArray[0]); // 1
console.log(nombreArray[1]); // 2
```

Un índice que no existe en un array devuelve `undefined`.

## Propiedades

- `length`: Devuelve la longitud de un array.

```javascript
let nombreArray = [1, 2, 3, 4, 5];
console.log(nombreArray.length); // 5
```
- `forEach()`: Ejecuta una función por cada elemento de un array.

```javascript
let nombreArray = [1, 2, 3, 4, 5];
nombreArray.forEach(function(elemento) {
    console.log(elemento);
});
```
- `push()`: Añade un elemento al final de un array.

```javascript
let nombreArray = [1, 2, 3, 4, 5];
nombreArray.push(6);
console.log(nombreArray); // [1, 2, 3, 4, 5, 6]
```
- `pop()`: Elimina el último elemento de un array.

```javascript
let nombreArray = [1, 2, 3, 4, 5];
nombreArray.pop();
console.log(nombreArray); // [1, 2, 3, 4]
```
- `shift()`: Elimina el primer elemento de un array.

```javascript
let nombreArray = [1, 2, 3, 4, 5];
nombreArray.shift();
console.log(nombreArray); // [2, 3, 4, 5]
```
- `unshift()`: Añade un elemento al principio de un array.

```javascript
let nombreArray = [1, 2, 3, 4, 5];
nombreArray.unshift(0);
console.log(nombreArray); // [0, 1, 2, 3, 4, 5]
```
- `indexOf()`: Devuelve el índice de un elemento en un array.

```javascript
let nombreArray = ['Pepe', 'Carlos', 'Raúl', 'David', 'Iván'];
console.log(nombreArray.indexOf('David')); // 3
```
- `splice()`: Añade o elimina elementos de un array.
```javascript
let nombreArray = ['Pepe', 'Carlos', 'Raúl', 'David', 'Iván'];
nombreArray.splice(2, 1);
console.log(nombreArray); // ['Pepe', 'Carlos', 'David', 'Iván']
```
```javascript
let nombreArray = ['Pepe', 'Carlos', 'Raúl', 'David', 'Iván'];
nombreArray.splice(2, 0, 6, 7);
console.log(nombreArray); // ['Pepe', 'Carlos', 6, 7, 'Raúl', 'David', 'Iván']
```
  - Explicación de cada parámetro:
    - `2`: Índice donde se va a añadir o eliminar elementos.
    - `0`: Número de elementos a eliminar.
    - `6, 7`: Elementos a añadir.