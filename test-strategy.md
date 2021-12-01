Listado del testeo y correciones:

1. la Función guessSubmit.addeventListener no es una función, error en la linea 87.
	
	Solución, la función esta mal escrita se corrigió con lo siguiente 
	guessSubmit.addEventListener 

2. No se pueden establecer propiedades de nulo (configurando 'textContent') linea 79.

	Solución, en la linea 50 en el document.querySelector estaba de la siguiente manera
	document.querySelector('lowOrHi') se solucionó agregando un punto al selector de la 
	siguiente manera document.querySelector('.lowOrHi')

3. la Función resetButton.addeventListener no es una función, error en la linea 96.

	Solución, la función esta mal escrita se corrigió con lo siguiente 
	resetButton.addEventListener

4. El programa no tira una alerta cuando se ingresa un numero no entero.

	Se agrego una condición para validar el ingreso de números para que solo acepte números enteros.


5. El programa no contiene una condición para válidar si un número esta en el rango de 1 - 100.

	Se agrego una condición para validar el ingreso de números para que cumpla con el rango de 1 - 100
	en la función checkGuess

6. El programa termina cuando era el 5to. intento y decía que había ganado el usuario.

	Solución: a la variable ATTEMPS se le asigno el 10 para validar el número de intentos que puede
	adivinar el usuario.

7. Dentro del código estaba mal validado cuando termina el juego cuando llega a 10 intentos y el usuario
   adivino el número. Las condiciones estaban alreves.
	
	Solución. se intercambiaron las condiciones cuando termina el juego cuando el usuario hace 10
	intentos y cuando el usuario seleccion el número correcto.

8. El número aleatorio incorrecto.

	solución. Se creo una función para que el numero aleatorio estuviera entre 1 y 100, al mismo tiempo
	que número sea entero.

9. En la linea 74 en la condición donde válida si el usuario adivino el número, se cambio el operador === a ==
   porque la variable pueden ser de diferentes tipos, la variable que ingresa el usuario es de tipo
   String y la variable que esta en el sistema es de tipo int