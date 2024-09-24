## Formas de declarar un String

`const producto = 'monitor' `-> primitiva
`const producto2 = String('monitor de 24 pulgadas')`
`const producto3 = new String('Monitor de 50 pulgadas') `-> se muestra en consola como un objeto, dando su longitud y diferentes parámetros

`console.log(producto3)`

## Metodos que puedo heredar de String

### replace, slice, substring y chartAt

`const producto = "monitor de 20 pulgadas"`

-> replace:
	`console.log(producto.replace("20","24"))`
	`console.log(producto.replace("pulgadas",' " '))`

-> slice:
	`console.log(producto.slice(0,10));`
	`console.log(producto.slice(2,10));`
	`console.log(producto.slice(2,1));  ` -> en este caso no corta hacia atras, no saldria nada por consola!!

-> substring
	`console.log(producto.substring(0,10))` -> desde la posición 0, hasta la 10
	`console.log(producto.substring(2,1))` -> ordena los dos argumentos desde 2 hasta 1

-> chartAt
	`const nombre = 'Juan';`
	`console.log(nombre.chatAt(0)) `-> devuelve el caracter de la posición 0, en este caso 'J'


### repeat y split

-> repeat:
	`const producto = 'monitos de 20 pulgadas';`
	`const texto = "en oferta".repeat(3); `-> repetiria seguido "en oferta"
	`console.log('$(producto)$(texto)')`-> se concatenan

-> split: divide la cadena, devuelve un array de cada string
	`const actividad = "Estamos revisando los fundamentos de JS"`
	`console.log(actividad.split(" "))` -> separa por cada espacio en blanco

### upperCase, lowerCase y toString

` const producto = "monitor 20 pulgadas"`

-> .toUpperCase()
	`console.log(producto.toUpperCase())

-> .toLowerCase()
	`console.log(producto.toLowerCase())

-> .toString()
	`const producto = 20;
	`console.log(producto.toString())