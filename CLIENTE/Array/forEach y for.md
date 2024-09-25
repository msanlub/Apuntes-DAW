

```
const carrito = [
	{name: "raton",price:30},
	{name: "tele",price:55},
	{name: "pc",price:185},
	{name: "mesa",price:60}
]

for (let i=0; i < carrito.lenght; i++){
	console.log('articulo: ${carrito[i].name} Precio: euros ${carrito[i].price}')
}


-------------------------------------------
carrito.forEach(function (producto) {
	console.log('articulo: ${producto.name} Precio: euros ${producto.price}')
})
```