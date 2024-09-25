```
const producto = {
	name: "Teclado",
	price: 20,
	available: true,
	"estado producto": "disponible"
}

//asignamos una propiedad a una variable
let name = producto.name

// es igual que hacer: let { propiedad } = nombreObjeto
let { name } = producto;

console.log(name)

//extraer mas de uno
let { name, price } = producto;

console.log(name)
console.log(price)

```

Para extraer cualquier propiedad debe estar definida previamente en el objeto.

Para destructurar un objeto anidado:

```
const producto = {
	name: "Teclado",
	price: 20,
	available: true,
	information: {
		peso: "1kg",
		medida: "20 cm",
		origin: {
			pais: "ES"
			}
	}
}

//forma normal
console.log(producto)
console.log(producto.information)
console.log(producto.information.peso)
console.log(producto.information.origin.pais)

//destructurar 
let { price, information: {origin} } = producto

console.log(origin) -> sacaria con este nombre la variable, no con information


let { information: {origin: {pais}}} = producto
console.log(pais)


```