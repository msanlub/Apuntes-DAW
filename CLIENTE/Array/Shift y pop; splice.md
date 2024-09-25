Para eliminar elementos de un array:

 
```
const producto1 = {
name: "raton",
price: 30,
}

const producto2 = {
name: "teclado",
price: 20,
}

const producto3 = {
name: "mesa",
price: 430,
}

carrito.push(producto1)
carrito.push(producto2)
carrito.unshift(producto3)



carrito.shift() //elimina el primer elemento
carrito.pop() // elimina el ultimo


//OTRA MANERA

carrito.splice(1,1) //solo el elemento 1
o
carrito.splice(1,3) //desde el elemento 1 hasta el 3

```