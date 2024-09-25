Otra forma de "congelar" el objeto, sin poder añadir o eliminar propiedades pero si modificando las ya creadas de antes: 

```
"use strict"
const producto = {
	name: "Teclado",
	price: 20,
	available: true,
	"estado producto": "disponible"
}

Object.seal(producto)

producto.color = "verde" -> saltaría error
producto.name = "coche" -> estaría correcto

```