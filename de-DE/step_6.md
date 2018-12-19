## Den Schwierigkeitsgrad steigern

Lass uns das Spiel noch schwieriger gestalten, je länger der Spieler am Leben bleibt, indem wir langsam die Verzögerung zwischen dem Erscheinen der Punkte drosseln.

+ Erstelle eine neue Variable namens`delay`{:class="blockdata"} (Verzögerung).

+ Erstelle nun in deinem Stadium ein neues Script, welches die Verzögerung auf eine hohe Zahl einstellt und dann langsam diese Verzögerungszeit drosselt.

	```blocks
		Wenn die grüne Flagge angeklickt
		setze [delay v] auf (8)
		wiederhole bis <(delay) = (2)>
  			 warte (10) Sek.
  			 ändere [delay v] um (-0.5)
		Ende
	```

	Merkst du, dass dies sehr ähnlich wie eine Spielzeituhr funktioniert?

+ Abschließend kannst du diese `delay`{:class="blockdata"} (Verzögerung) Variable in deinen roten, gelben und blauen Punkten Scripts benutzen. Entferne den Code, der eine zufällig ausgewählte Zahl an Sekunden zwischen dem Erstellen von Klonen wartet und ersetze ihn mit deiner neuen `delay`{:class="blockdata"} (Verzögerung) Variable:

	```blocks
		warte (delay) Sek.
	```

+ Teste deine neue `delay`{:class="blockdata"} (Verzögerung) Variable und schau, ob die Verzögerung zwischen den einzelnen Punkten langsam gesenkt wird. Funktioniert dies bei allen 3 der bunten Punkte? Kannst du den Wert der `delay`{:class="blockdata"} (Verzögerung) Variable sehen, wie er sich senkt?


