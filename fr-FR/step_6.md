## Augmentation de la difficulté

Créons un jeu qui devient de plus en plus difficile quand joueur survit plus longtemps, en réduisant l'écart entre l'apparition des points.

+ Créez une nouvelle variable appelée `écart`{:class="blockdata"}.

+ Sur votre étape, créez un nouveau script qui rend l'écart à un chiffre élevé et qui réduit ensuite lentement le temps d'écart.

	```blocks
		quand le drapeau vert pressé
		mettre [delay v] à (8)
		répéter jusqu’à <(delay) = (2)>
   			attendre (10) secondes
   			ajouter à [delay v] (-0.5)
		fin
	```

	Remarquez que c'est semblable au fonctionnement d'une minuterie !

+ Finalement, vous pouvez utiliser cette variable `écart`{:class="blockdata"} dans les scripts de vos points rouges, jaunes et bleues. Enlevez le code qui attend un nombre de secondes aléatoires pour créer des clones et remplacez-le par votre nouvelle variable `écart`{:class="blockdata"}:

	```blocks
		attendre (retard) secondes
	```

+ Testez votre nouvelle variable `écart`{:class="blockdata"} et regardez si le retard entre les points réduit lentement. Est-ce que cela fonctionne pour les 3 points colorés ? Pouvez-vous voir la valeur de l' `écart`{:class="blockdata"} réduire ?
