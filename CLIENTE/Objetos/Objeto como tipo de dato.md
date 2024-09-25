### Crear y acceder a los valores de un objeto


```
const producto = {
	name: "Teclado",
	price: 20,
	available: true,
	"estado producto": "disponible"
}


//accedo al objeto
console.log(producto)
console.log(producto.name)
console.log(producto["name"])
console.log(producto["estado producto"]) 

//añadir propiedad
producto.color = "verde"

//eliminar propiedades
delete producto.price
console.log(producto)

```


Para acceder a un valor con un nombre compuesto como "estado producto" hay que hacerlo con [" "], es la manera antigua de hacerlo JS.


Aunque un objeto sea constante, se le puede añadir o eliminar propiedades. Hay formas de hacer que un objeto sea inmutable ( otro fichero).