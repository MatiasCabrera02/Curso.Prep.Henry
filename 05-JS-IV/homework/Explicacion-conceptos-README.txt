Explicación de los conceptos de: *Objetos, *Propiedades, *Métodos, *Bucle for...in, *Dot Notation(notación de puntos) y *Brackets notation(notación de corchetes).

Objetos:
	  Los objetos son muy similares a los arrays, almacenan mucha cantidad de información pero sobre una cosa en particular (los arrays sobre diferentes cosas sin estar precisamente relacionado). Se basa en una sintaxis de key:value (propiedad:valor) y los objetos se crean:
var objeto = {
	key:value;}.

Propiedades:
		Las propiedades son las palabras claves a las que se les asignan valores, las key.

Métodos:
	  Los métodos en los objetos son las funciones (function) como valores en los pares clave:valor.

Loop for...in:
		  Este bucle sirve para iterar en los pares clave:valor. Su sintaxis es: for(var clave in objeto) en donde es muy similar al bucle for, aquí luego de declarada la variable var/let sigue la palabra clave/propiedad del objeto, luego la palabra clave IN y por último el nombre del objeto. Sirve para recorrer todas las claves y finalizará cuando se hayan iterado todas las mismas. Ej: for(var clave in objeto){console.log(clave); console.log(usuario[clave]);}

Dot notation vs Bracket notation:
		 			   Ámbos sirven para la misma tarea, ya sea acceder a valores o asignar valores a un objeto, dependerá de c/u cual elegir, pero generalmente los corchetes se usan con variables.
Para acceder con la notación de punto se hace: primero llamamos al nombreObjeto.nombreClave // 12345

Por otro lado, con la notación de corchetes es como llamar un elemento a una matriz, aunque con corchetes se debe usar una cadena o número, o una variable que apunte a una cadena o número, se puede llamar a cada clave envolviéndola en comillas: nombreObjeto["nombreClave"]; // 12345
(si es variable no hace falta "").

Para otra cosa que sirven es para asignar valores y funciona igual que acceder:

Dot notation: nuevoUsuario.username = "otro.nombre.usuario";

Bracket notation: nuevoUsuario["password"] = "12345";

O si es una variable: nuevoUsuario[loveJSString] = true;

(También se pueden asignar valores cuando creamos el objeto)