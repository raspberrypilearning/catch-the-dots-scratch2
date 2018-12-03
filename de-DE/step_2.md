## Einen Controller herstellen

Lass uns damit beginnen, einen Controller herzustellen, der dazu benutzt wird, um die Punkte einzufangen.

+ Öffne das 'Catch the Dots' (Fang die Punkte) Scratch Projekt online unter <a href="http://jumpto.cc/dots-go" target="_blank">jumpto.cc/dots-go</a> oder lade es von <a href="http://jumpto.cc/dots-get" target="_blank">jumpto.cc/dots-get</a> herunter udn öffnes es dann, wenn du den offline Editor benutzt.

	Du solltest ein Controller Sprite sehen können:

	![screenshot](images/dots-controller.png)
	
	
+ Drehe deinen Controller nach rechts, wenn die rechte Pfeiltaste gedrückt wird:

	```blocks
		Wenn die grüne Flagge angeklickt
		wiederhole fortlaufend
  			 falls <Taste [Pfeil nach rechts v] gedrückt?> dann
      			drehe dich nach rechts um (3) Grad
   			Ende
		Ende
	```
+ Teste deinen Controller: Er sollte sich nach rechts drehen.


