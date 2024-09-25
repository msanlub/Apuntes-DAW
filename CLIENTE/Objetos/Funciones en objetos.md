
```
"use strict"
name = "raton"
price = 30

const producto = {
	name: "Teclado",
	price: 20,
	available: true,
	mostrarInfo: function(){
		console.log('${name});
		console.log(`${price});
	}
}

producto.mostrarInfo()
//esto mostraria raton y 30, para que enseñe teclado y 20 debo usar this

const producto = {
	name: "Teclado",
	price: 20,
	available: true,
	mostrarInfo: function(){
		console.log('${this.name});
		console.log(`${this.price});
	}
}
```