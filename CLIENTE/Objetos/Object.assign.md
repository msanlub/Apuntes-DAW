Para unir objetos, creando copias y manteniendo los objetos:

```
"use strict"
const producto = {
	name: "Teclado",
	price: 20,
	available: true,
	"estado producto": "disponible"
}

const medidas = {
	peso: "1kg",
	medida: "1m",
}

const medidas1 = {
	peso1: "4kg",
	medida1: "5m",
}

console.log(producto)
console.log(medidas)

// assign
const resultado = Object.assign(producto,medidas,medidas1)

console.log(resultado
)

```

