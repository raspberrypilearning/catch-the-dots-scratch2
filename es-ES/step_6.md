## Aumentar la dificultad

Vamos a hacer que el juego sea más difícil cuanto más tiempo consiga sobrevivir el jugador, reduciendo lentamente el intervalo entre los puntos que aparecen.

+ Crea una nueva variable con el nombre `intervalo`{:class="blockdata"}.

+ En el escenario, crea nuevo código que fije el intervalo en un número alto, y que lentamente vaya reduciendo el valor del intervalo.

	```blocks
		al presionar bandera verde
		fijar [intervalo v] a (8)
		repetir hasta que <(intervalo) = (2)>
   			esperar (10) segundos
   			cambiar [intervalo v] por (-0.5)
		fin
	```

	¡Fíjate que esto es muy parecido a cómo funciona un cronómetro en el juego!

+ Para acabar, puedes utilizar la variable `intervalo`{:class="blockdata"} en el código de tus puntos rojo, amarillo y azul. Elimina el código que espera un número al azar de segundos para crear clones, y sustitúyelo con tu nueva variable `intervalo`{:class="blockdata"}:

	```blocks
		esperar (intervalo) segundos
	```

+ Prueba tu nueva variable `intervalo`{:class="blockdata"}, y comprueba si el intervalo entre los puntos se reduce lentamente. ¿Funciona para los 3 puntos de colores? ¿Puedes ver cómo se reduce el valor de la variable `intervalo`{:class="blockdata"}?



