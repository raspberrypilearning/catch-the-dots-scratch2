## Moeilijker maken

We gaan het spel moeilijker maken naarmate de speler langer overleeft, door de vertraging tussen het verschijnen van stippen langzaam kleiner te maken.

+ Maak een nieuwe variabele met de naam `vertraging`{:class="blockdata"}.

+ Maak in het speelveld een ​​nieuw script met de vertraging op een hoog getal en verminder daarna langzaam de vertragingstijd.
    
```blocks
wanneer groene vlag wordt aangeklikt
maak [vertraging v] (8)
herhaal tot <(vertraging) = (2)> 
  wacht (10) sec.
  verander [vertraging v] met (-0.5)
end
```

Merk op dat dit erg lijkt op hoe een speltimer werkt!

+ Ten slotte kunt je de variabele `vertraging`{: class = "blockdata"} gebruiken in de scripts van de rode, gele en blauwe stippen. Verwijder de code die een willekeurig aantal seconden wacht tussen het maken van klonen en vervang dat door de nieuwe `vertraging`{:class="blockdata"} variabele:
    
```blocks
wacht (vertraging) sec.
```

+ Test de nieuwe `vertraging`{:class="blockdata"} -variabele en kijk of de vertraging tussen de stippen langzaam afneemt. Werkt dit voor alle 3 gekleurde stippen? Kun je zien dat de waarde van de `vertraging`{:class="blockdata"} -variabele vermindert?