## Creare un controller

Iniziamo con il creare un controller che può essere usato per raccogliere i puntini.

+ Apri il progetto Scratch online 'Acchiappa Puntini' a <a href="http://jumpto.cc/dots-go" target="_blank">jumpto.cc/dots-go</a> o scaricalo da <a href="http://jumpto.cc/dots-get" target="_blank">jumpto.cc/dots-get</a> e poi apri se stai usando l'editore offline.

	Dovresti vedere lo sprite di un controller:

	![screenshot](images/dots-controller.png)


+ Gira il controller a destra quando la freccia destra è premuta:

	```blocks
		quando si clicca sulla bandiera verde
		per sempre
  			se <tasto [freccia destra v] premuto> allora
   				ruota in senso orario di (3) gradi
  			end
		end
	```
+ Testa il tuo controller -- dovrebbe ruotare verso destra.

