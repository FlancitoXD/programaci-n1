## programacion 1

## descripcion
taller de programacion 1 - 5to com B
## Temas Trabajadores:
-selectivas
-repetitivas
-arreglos -> simples y compuestos
P.O.O -> Clases, Subclases, Objetos y Pilares
-DOM

##
-Selectivas
el if y else funcionan para que el programa tome decisiones mediante una condicional
```bash
// IF básico

if (nota >= 6) {

  console.log("Aprobaste");

}


// IF / ELSE

if (nota >= 6) {

  console.log("Aprobaste ✅");

} else {

  console.log("Reprobaste ❌");

}


// IF / ELSE IF / ELSE → evalúa de ARRIBA HACIA ABAJO

// Entra en el PRIMER bloque que sea true. Las demás se ignoran.

if (nota === 10) {

  console.log("Sobresaliente");

} else if (nota >= 7) {

  console.log("Muy bueno");    // nota 7 → entra acá y PARA

} else if (nota >= 6) {

  console.log("Aprobado");     // nunca llega, aunque 7 >= 6

} else {

  console.log("Reprobado");

}
```
##
-repetitivas
El do while es una estructura repetitiva que permite ejecutar un bloque de código varias veces mientras se cumpla una condición.
La diferencia principal con el while es que el do while ejecuta el código al menos una vez, aunque la condición sea falsa.
```bash
let x = 5;


do {

  console.log("x vale: " + x);

  x++;

} 

while (x < 3);


// x=5 → condición false desde

// el inicio, pero igual ejecuta

// una vez y muestra: 'x vale: 5'
```

##
-arreglos -> simples y compuestos


arreglo simple
En programación, un arreglo es un conjunto de datos que se almacenan bajo un mismo nombre.
```bash
const vacio = [];


const frutas = ["manzana", "banana", "naranja"];


// Acceder por índice


console.log(frutas[0]);  // "manzana"


console.log(frutas[2]);  // "naranja"


// Modificar un elemento


frutas[1] = "pera";


console.log(frutas);
```

arreglo compuesto
Es una estructura que permite agrupar diferentes tipos de datos en un variable
```bash
let productos = [
 { id: 1, nombre: "Pera", precio: 1500, stock: 20 },
 { id: 2, nombre: "Manzana", precio: 2200, stock: 0 },
 { id: 3, nombre: "Banana", precio: 1800, stock: 15 },
 { id: 4, nombre: "Frutilla", precio: 3500, stock: 5 },
 { id: 5, nombre: "Naranja", precio: 1200, stock: 0 }
];
let disponibles = productos.filter((p)=> p.stock > 0)
console.log(disponibles)
let prodCompleto = productos.find((p)=> p.id === 4)
console.log(prodCompleto)
let newLista = productos.map((p)=>console.log(`Producto:${p.nombre}-$${p.precio}`))
let produmenos2k = productos.filter((p)=> p.precio<2000)
console.log(produmenos2k.length)
}
```

##
-P.O.O -> Clases, Subclases, Objetos y Pilares
La POO (Programación Orientada a Objetos) es una forma de programar que organiza el código mediante objetos que tienen características y funciones.
```bash
class Celular {
    //marca, modelo, color, bateria, camaras, funda, pantalla.
    #pin;
    #intento
    #bloqueo
    constructor(marca, modelo, bateria, pin, ) {
        this.marca = marca;
        this.modelo = modelo;
        this.bateria = bateria;
        this.#pin = pin;
        this.#intento = 0;
        this.#bloqueo = false;
    }
 }
```

##
-DOM
El DOM (Document Object Model) es una estructura que permite a los lenguajes de programación acceder, modificar y manipular los elementos de una página web, como títulos, imágenes, textos y botones.
- JS:
```bash
let titulo = document.createElement("h1");
titulo.textContent = "¡Hola Mundo!"
titulo.classList.add("titulo");
```

- HTML:
```bash

<h1>¡Hola Mundo!</h1>
```

- CSS:
```bash
.titulo{
color: pink;
}
```
