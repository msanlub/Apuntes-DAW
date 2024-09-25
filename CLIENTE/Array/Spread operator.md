
Para añadir elementos al array

```
const carrito = []

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

let resultado;
resultado = [...carrito, producto1]
resultado = [...resultado, producto2]
resultado = [producto3,...resultado]

console.log(resultado)
```

La diferencia entre spread y  push y unshift es que spread crea una copia del elemento inicial que es la forma declarativa, la imperativa no hace una copia del elemento original, la declaratia es más funcional(spread operator).