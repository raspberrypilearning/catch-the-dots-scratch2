## Punkte einsammeln

Lass uns ein paar Punkte hinzufügen, die der Spieler mit dem Controller einsammeln kann.

+ Erstelle ein neues Sprite namens 'red' (rot). Dieses Sprite sollte ein kleiner roter Punkt sein.

	![screenshot](images/dots-red.png)

+ Füge dieses Script zu deinem 'red' roten Punkt Sprite hinzu, um alle paar Sekunden einen neuen Punkt-Klon zu erstellen:

	```blocks
		Wenn die grüne Flagge angeklickt
		verstecke dich
		warte (2) Sek.
		wiederhole fortlaufend
  			 erzeuge Klon von [mir selbst v]
  			 warte (Zufallszahl von (5) bis (10)) Sek.
		Ende
	```

+ Wenn jeder Klon erstellt wurde, willst du, dass er in einer der 4 Ecken des Stadiums erscheint.

	![screenshot](images/dots-start.png)

	Damit dies geschieht, musst du als erstes eine neue __Liste__ namens `start positions`{:class="blockdata"} (Startpositionen) erstellen und auf das `(+)` klicken, um die Werte `-180` und `180` hinzuzufügen.

	![screenshot](images/dots-list.png)

+ Du kannst diese 2 Listen-Artikel benutzen, um eine zufällige Ecke des Stadiums auszuwählen. Füge diesen Code zum 'dot' (Punkt) Sprite hinzu, sodass jeder neue Klon sich in eine zufällig ausgewählte Ecke bewegt und sich dann langsam auf den Controller zubewegt.

	```blocks
		Wenn ich als Klon entstehe
		gehe zu x:(Element (random v) von [start positions v]) y:(Element (random v) von [start positions v])
		drehe dich zu [controller v]
		zeige dich
		wiederhole bis <wird [controller v] berührt?>
   			gehe (1) er-Schritt
		Ende
	```

	Der o.g. Code wählt entweder `-180` oder `180` für die x _und_ y Positionen, was bedeutet, dass jeder Klon in einer Ecke des Stadiums beginnt.

+ Teste dein Projekt. Du solltest jetzt sehen können, dass ganz viele rote Punkte in jeder Ecke des Bildschirms erscheinen und sich langsam auf den Controller hinzubewegen.

	![screenshot](images/dots-red-test.png)

+ Erstelle 2 neue Variable namens `lives`{:class="blockdata"} (Leben) und `score`{:class="blockdata"} (Punktzahl).

+ Füge den Code zu deinem Stadium hinzu, um die `lives`{:class="blockdata"} Leben-Blockdaten auf 3 und die `score`{:class="blockdata"} Punktzahl-Blockdaten auf 0 zu Beginn des Spiels einzustellen.

+ Du musst den Code zum Ende deines roten `when I start as a clone`{:class="blockcontrol"} (wenn ich als Klon beginne) Punkt-Codes hinzufügen, damit entweder 1 zur `score`{:class="blockdata"} (Punktzahl) des Spielers hinzugefügt wird, wenn die Farben zueinander passen oder 1 vom `lives`{:class="blockdata"} Leben des Spielers abgezogen wird, wenn die Farben nicht zueinander passen.

	```blocks
		gehe (5) er-Schritt
		falls <wird Farbe [#FF0000] berührt?> dann
   			ändere [score v] um (1)
   			spiele Klang [pop v]
		sonst
  			ändere [lives v] um (-1)
   			spiele Klang [laser1 v]
		Ende
		lösche diesen Klon
	```

+ Füge diesen Code zum Ende deines Stadion-Scripts hinzu, damit das Spiel beendet wird, wenn der Spieler alle seine Leben verloren hat:

	```blocks
		warte bis <(lives) < [1]>
		stoppe [alles v]
	```

+ Teste dein Spiel, um zu gewährleisten, dass dieser Code wie erwartet funktioniert.
