## Aumenta la difficoltà

Aumentiamo la difficoltà del gioco man mano che il giocatore continua a  sopravvivere, riducendo lentamente il ritardo di comparsa tra i puntini.

+ Crea una nuova variabile chiamata `ritardo`{:class="blockdata"}.

+ Sul tuo quadro, crea un nuovo testo che imposti il ritardo a un numero alto, e riduca poi il tempo di ritardo.

	```blocks
		quando si clicca sulla bandiera verde
		porta [ritardo v] a (8)
		ripeti fino a quando <(ritardo) = (2)>
  			attendi (10) secondi
  			cambia [ritardo v] di (-0.5)
		end
	```

	Nota che è molto simile al modo di funzionare di un timer!

+ Infine, puoi usare questa variabile `ritardo`{:class="blockdata"} nei testi dei tuoi puntini rossi, gialli e blu. Rimuovi il codice che aspetta un numero di secondi a caso nella creazione dei cloni, e sostituiscilo con la tua nuova variabile `ritardo`{:class="blockdata"}:

	```blocks
		attendi (ritardo) secondi
	```

+ Prova la tua nuova variabile `ritardo`{:class="blockdata"}, e vedi se il ritardo tra i puntini si riduce lentamente. Funziona per tutti e 3 i puntini colorati? Vedi che il valore della variabile `ritardo`{:class="blockdata"} si riduce?
