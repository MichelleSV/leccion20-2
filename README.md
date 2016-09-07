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
Al principio tenemos una funcion autoejecutable, por lo cual, al ejecutarse tomará la variable local que se le ha trogado
