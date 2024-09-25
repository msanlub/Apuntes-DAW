
Desestructurar el array:

```
const numeros = [10,20,30,40]

const [primer,sgundo,tercero] = numeros
console.log(primer)
console.log(sgundo)
console.log(tercero)

//solo el segundo
const [, sgundo] = numeros
console.log(sgundo)


const numeros = [10,20,30,40,56,70]

const [primer, sgundo, ...resto] = numeros
console.log(resto) -> los otros 4 elementos restantes

```