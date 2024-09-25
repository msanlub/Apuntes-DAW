
Para que no se pueda modificar un objeto:


```
"use strict"
const producto = {
	name: "Teclado",
	price: 20,
	available: true,
	"estado producto": "disponible"
}

Object.freezee(producto) -> se congela el objeto producto

//comprobamos el freeze
console.log(object.isFrozen(pdoructo)) -> true

producto.available = false
console.log(producto)

```

Con uso estricto accedemos al uso moderno de JS, entonces salta error cuando quiero modificar una propiedad una vez usado el Object.freezee, funcion heredada del objeto Object.