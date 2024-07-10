# Principales acciones de JavaScript sobre el DOM

- `document.getElementById()`: Permite seleccionar un elemento por su id.
```javascript
var boton = document.getElementById('boton');
boton.innerHTML = 'Nuevo texto del botón';
```
- `document.getElementsByClassName()`: Permite seleccionar un elemento por su clase.
- `document.getElementsByTagName()`: Permite seleccionar un elemento por su etiqueta.
```javascript
var h1 = document.getElementsByTagName('h1');
h1[0].innerHTML = 'Nuevo título';
```

- `document.createElement()`: Permite crear un elemento.
- `parentNode.appendChild()`: Permite agregar un elemento al final de otro.
- `element.innerHTML`: Permite obtener o cambiar el contenido de un elemento.
- `element.style.left`: Permite obtener o cambiar la propiedad left de un elemento.
- `element.setAttribute()`: Permite agregar un atributo a un elemento.
- `element.getAttribute()`: Permite obtener el valor de un atributo de un elemento.
- `element.addEventListener()`: Permite agregar un evento a un elemento.
```javascript
boton.addEventListener('click', mensaje);
function mensaje() {
    alert('Mensaje de prueba');
}
// Al clicar el botón, se mostrará un mensaje de alerta
```
- `window.content`: Permite obtener el contenido de la ventana.
- `window.onload`: Permite ejecutar una función cuando la ventana se ha cargado.
- `window.dump()`: Permite mostrar un mensaje en la consola.
- `window.scrollTo()`: Permite desplazar la ventana a una posición específica.
- `document.title`: Permite obtener o cambiar el título de la página.
```javascript
console.log(document.title) // Muestra el título de la página
document.title = 'Nuevo título' // Cambia el título de la página
console.log(document.title) // Muestra el nuevo título de la página
```