Para unir objetos, crea copias de cada objeto,asi se mantienen y las une

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

const resultado2 = {...producto, ...medidas}

console.log(resultado2)
```