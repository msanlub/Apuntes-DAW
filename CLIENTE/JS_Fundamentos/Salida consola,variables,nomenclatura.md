## Salida por consola

| Comando                                 | Descripción                                                            |
| --------------------------------------- | ---------------------------------------------------------------------- |
| `console.log('Esto sale por consola');` | Muestra un mensaje en la consola.                                      |
| `console.table([1,2,3,4,5]);`           | Muestra una tabla en la consola con el array.                          |
| `console.time("Hola")`                  | Cuenta el tiempo que tarda en ejecutarse el código hasta poner timeEnd |
| `console.warn("ALERTA")`                | Muestra mensaje como alerta                                            |
| `console.timeEnd("Hola")`               | Sale el tiempo que ha tardado en ejercutarse desde el time de antes.   |

## Variables

| var                                    | let                                    | const                                    |
| -------------------------------------- | -------------------------------------- | ---------------------------------------- |
| Se puede cambiar, no aconsejable       | Se puede cambiar                       | Es una constante, no cambia              |
| `var producto = "Monitor 10 pulgadas"` | `let producto = "Monitor 20 pulgadas"` | `const producto = "Monitos 20 pulgadas"` |
| `producto = "Monitor sin pulgadas"`    | `producto = "Monitor sin pulgadas"`    |                                          |
| `producto = 20(se conviente a Int)`    | ` producto = 20(se conviente a Int)`   |                                          |

* Para iniciar multiples variables separo con comas, no hace falta poner el var:
	`var categoria = "pc",
	`marca = "logitech",
	`calificación = 2 ;`


## Nomenclatura JavaScript

`let nombreproducto = "monitor" 
`let nombreProducto = "monitor" `-> CamelCase
`let nombre_producto = "monitor" `-> underscore
`let NombreProducto = "monitor" `->PascalCase