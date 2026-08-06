***
+ **Das Beispiel** (nicht gelabelt): 
	+ Datensatz ist Sammlung nicht gelabelter Beispiele $\{x_i\}_{i=1}^N$
	+ Jedes Element **$x_i$** im Datensatz wird **feature vector** genannt.
+ **Ziel**
	+ Algorithmus des unsupervised learning dient dazu, ein Modell zu erstellen, das einen **feature vector $x_i$** als Eingabe entgegennimmt und diesen entweder **in einen anderen Vektor oder in einen Wert umwandelt, der zur Lösung eines praktischen Problems verwendet werden kann.**
	+ Beispiel: 
		+ Das Modell leifert beim Clustering für jeden Merkmalsvektor im Datensatz die ID des Clusters zurück. Bei der Dimensionsreduktion ist die Ausgabe des Modells ein Merkmalsvektor, der weniger Merkmale enthält als die Eingabe $x$. Bei der Ausreißererkennung ist die Ausgabe eine reelle Zahl, die angibt, inwiefern sich $x$ von einem „typischen“ Beispiel im Datensatz unterscheidet.

