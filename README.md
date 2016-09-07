# Ejercicio 2
### Código inicial
```js
var feature = 'closures'; 
(function () {     
	if ( typeof feature === 'undefined' ){         
		var feature = 'callbacks';         
		console.log('JS coders love its ' + feature );     
	} else {         
		console.log('JS developers love its ' + feature );     
	} 
})();
```

### Solución planteada 
```js
var feature = 'closures'; 
(function () {     
	if ( typeof feature === 'undefined' ){         
		feature = 'callbacks';         
		console.log('JS coders love its ' + feature );     
	} else {         
		console.log('JS developers love its ' + feature );     
	} 
})();
```
En una funcion autoejecutable corre primero el código que está dentro y al momento de correr usa su variable local, entonces, al momento de borrar el "var" de la variable local, la convertimos en global y por lo tanto la funcion toma la primera variable global para ejecutarse. Esto pasa debido  al comportamiento predeterminado del movimiento de JavaScript(hoisting).
