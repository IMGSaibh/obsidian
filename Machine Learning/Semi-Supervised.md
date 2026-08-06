***
+ **Das Beispiel** (nicht gelabelt): 
	+ Datensatz ist Sammlung nicht gelabelter Beispiele $\{x_i\}_{i=1}^N$
	+ Jedes Element **$x_i$** im Datensatz wird **feature vector** genannt.
+ Der Datensatz enthält sowohl **gelabelte** als auch **ungelabelte** Beispiele.
+ In der Regel ist die Anzahl der **gelabelte** Beispiele **deutlich höher** als die der **ungelabelte**
+ **Ziel**
	+  Des halbüberwachten Lernalgorithmus ist dasselbe **wie das Ziel eines überwachten Lernalgorithmus.** Dabei besteht die Hoffnung, dass die Verwendung vieler unbeschrifteter Beispiele dem Lernalgorithmus dabei helfen kann, ein besseres Modell zu finden (man könnte auch sagen: „zu erzeugen“ oder „zu berechnen“)[^1]

[^1]: Es mag widersinnig erscheinen, dass das Lernen davon profitieren könnte, wenn man weitere unbeschriftete Beispiele hinzufügt. Wenn man unbeschriftete Beispiele hinzufügt, fügt man mehr Informationen über das Problem hinzu: Eine größere Stichprobe spiegelt die Wahrscheinlichkeitsverteilung, aus der die von uns beschrifteten Daten stammen, besser wider. Theoretisch sollte ein Lernalgorithmus in der Lage sein, diese zusätzlichen Informationen zu nutzen.
