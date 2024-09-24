
### declarar numeros
`const numero = 1;`
`const numero2 = 2.2;`
`const numero3 = 0.5;
`const numero4 = .423;`

-> Declarar objeto numero 
`const numero6 = new Number(2);`


### operaciones
`const numero1 = 20;
`const numero2 = 10;`

`let resultado;`

->suma
	`resultado = numero1 + numero 2;
	
	console.log(resultado);
	
->resta
	`resultado = numero1 - numero2;
	
	console.log(resultado);
	
->multiplicación
	`resultado = numero1 * numero2;`
	
	console.log(resultado);
	
->division
	`resultado = numero1 / numero2;
	
	console.log(resultado);
	
->resto 
	`resultado = numero1 % numero2;
	
	console.log(resultado);


### Metodo Math

`let resultado

si hago un `console.log(Math)` me da todos los metodos que puedo usar
	
`console.log(Math.PI)` ->da el valor de pi
	
-> redondeo
	->round:  a partir de .5 redondea hacia arriba
		`resultado = Math.round(2.4)`
		`console.log(resultado)`-> devuelve 2
	->ceil: redondeo formado hacia arriba
		`resultado = Math.ceil(2.2)` 
		`console.log(resultado)`->fuerza redondeo hacia arriba (3)
	->floor: redondea hacia abajo
		`resultado = Math.floor(2.6)`
		console.log(resultado) -> fuerza redondeo hacia abajo (2)
	
-> raiz cuadrada
	`resultado = Math.sqrt(144)
	`console.log(resultado)
	
-> valor absoluto
	`resultado = Math.abs(-345)`->345 valor absoluto
	`console.log(resultado)
	
-> potencia
	`resultado = Math.pow(2,4)`->2⁴ = 16
	`console.log(resultado)
	
-> minimo
	`resultado = Math.min(3,5,6,7,1)`->1
	`console.log(resultado) 
	
->maximo
	`resultado = Math.max(3,5,6,7,1)`->7
	`console.log(resultado) 
	
->aleatorio
	`resultado = Math.random()`->numero aleatorio
	`resultado = Math.floor(Math.random()*30)` ->/de 0  a 30 redondeado
	
	console.log(resultado) 
	
->Orden
	
	let resultado
	resultado = 20 + 20 * 2;
	resultado = (20 + 20) * 2;
	
	console.log(resultado)
	
->Incremento
	`let puntuacion = 5;
	`console.log(puntuacion++)`-> muestra la variable y luego la incrementa, por lo que daria 5
	`console.log(++puntuacion) `-> esta si daria 6, incrementa y luego enseña
	
->decremento
	`console.log(puntuacion--)
	`console.log(--puntuacion)
	
	
->conversiones
	`const numero1 = "20";
	`const numero2 = "20.3";
	`const numero3 = "uno";
	`const numero4 = 20;
	`console.log(typeof(numero1));`-> String
	`console.log(typeof(numero4));`-> Number
	
-> convertir de String a Int
	`console.log(Number.parseInt(numero1)) `-> del objeto Number esta en la ventana global de JS, no hace falta ponerlo pero esta bien saber que usamos sus propiedades
	`console.log(Number.parseFloat(numero2))`-> 20.3
	`console.log(Number.parseInt(numero3))`-> Nan (not at number)
	
-> comprobar si un numero es entero
	`console.log(Number.isInteger(numero1))` -> false
	`console.log(Number.isInteger(numero4))` -> true
	
-> convertir un numero a string
	`console.log(numero4.toString())
	