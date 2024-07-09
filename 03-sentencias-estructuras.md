# Sentencia if..else

## Sentencia if

La sentencia `if` se utiliza para tomar decisiones basadas en condiciones.

```javascript
if (condición) {
    // Código a ejecutar si la condición es verdadera
}
```

Ejemplo:

```javascript
let edad = 18;

if (edad >= 18) {
    console.log('Eres mayor de edad');
}
```

## Sentencia if anidada

Se pueden anidar varias sentencias `if` dentro de otra.

```javascript
if (condición1) {
    // Código a ejecutar si la condición1 es verdadera
    if (condición2) {
        // Código a ejecutar si la condición2 es verdadera
    }
}
```

Ejemplo:

```javascript
let edad = 18;
let sexo = 'M';

if (edad >= 18) {
    if (sexo === 'M') {
        console.log('Eres mayor de edad y eres mujer');
    }
}
```

## Sentencia if..else

La sentencia `if..else` se utiliza para tomar decisiones basadas en condiciones. Si la condición es verdadera, se ejecuta el bloque de código dentro del `if`. Si la condición es falsa, se ejecuta el bloque de código dentro del `else`.

```javascript
if (condición) {
    // Código a ejecutar si la condición es verdadera
} else {
    // Código a ejecutar si la condición es falsa
}
```

Ejemplo:

```javascript
let edad = 15;

if (edad >= 18) {
    console.log('Eres mayor de edad');
} else {
    console.log('Eres menor de edad');
}
```

## Sentencia if..else if

La sentencia `if..else if` se utiliza para tomar decisiones basadas en varias condiciones. Si la primera condición es verdadera, se ejecuta el bloque de código dentro del `if`. Si la primera condición es falsa, se evalúa la siguiente condición. Si la segunda condición es verdadera, se ejecuta el bloque de código dentro del `else if`. Si la segunda condición es falsa, se ejecuta el bloque de código dentro del `else`.

```javascript
if (condición1) {
    // Código a ejecutar si la condición1 es verdadera
} else if (condición2) {
    // Código a ejecutar si la condición2 es verdadera
} else {
    // Código a ejecutar si ninguna de las condiciones es verdadera
}
```

Ejemplo:

```javascript
let edad = 15;

if (edad >= 18) {
    console.log('Eres mayor de edad');
} else if (edad >= 13) {
    console.log('Eres adolescente');
} else {
    console.log('Eres niño');
}
```

## Sentencia switch

La sentencia `switch` se utiliza para tomar decisiones basadas en varias condiciones. Se evalúa una expresión y se ejecuta el bloque de código correspondiente al caso que coincida con el valor de la expresión.

```javascript
switch (expresión) {
    case valor1:
        // Código a ejecutar si la expresión es igual a valor1
        break;
    case valor2:
        // Código a ejecutar si la expresión es igual a valor2
        break;
    default:
        // Código a ejecutar si la expresión no coincide con ningún caso
}
```

Ejemplo:

```javascript
let día = 'Lunes';

switch (día) {
    case 'Lunes':
        console.log('Hoy es lunes');
        break;
    case 'Martes':
        console.log('Hoy es martes');
        break;
    case 'Miércoles':
        console.log('Hoy es miércoles');
        break;
    case 'Jueves':
        console.log('Hoy es jueves');
        break;
    case 'Viernes':
        console.log('Hoy es viernes');
        break;
    case 'Sábado':
        console.log('Hoy es sábado');
        break;
    case 'Domingo':
        console.log('Hoy es domingo');
        break;
    default:
        console.log('Hoy no es un día de la semana');
}
```

# Bucle for

El bucle `for` se utiliza para repetir un bloque de código un número determinado de veces.

```javascript
for (inicialización; condición; actualización) {
    // Código a ejecutar en cada iteración
}
```

Ejemplo:

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

# Bucle while

El bucle `while` se utiliza para repetir un bloque de código mientras una condición sea verdadera.

```javascript
while (condición) {
    // Código a ejecutar en cada iteración
}
```

Ejemplo:

```javascript
let i = 0;

while (i < 5) {
    console.log(i);
    i++;
}
```

# Bucle do..while

El bucle `do..while` se utiliza para repetir un bloque de código al menos una vez y luego mientras una condición sea verdadera.

```javascript
do {
    // Código a ejecutar en la primera iteración
} while (condición);
```

Ejemplo:

```javascript
let i = 0;

do {
    console.log(i);
    i++;
} while (i < 5);
```

# Sentencias lógicas

Se pueden agrupar distintas condiciones utilizando operadores lógicos para ejecutar una estructura.

![Operadores lógicos](/img/03-operadores-logicos.png)