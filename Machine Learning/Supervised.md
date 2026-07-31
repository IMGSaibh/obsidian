***
+ **Das Beispiel** (später gelabelt): 
	+ Datensatz ist Sammlung von Beispielen die alle ein Label haben $\{(x_i, y_i)\}_{i=1}^{N}$
	+ Jedes Element **$x_i$** im Datensatz wird **[^1]feature vector** genannt. 
	+ jedes **feature** $x^{(j)}$ ist der der Wert einer Dimension des feature vectors
	+ Beispiel: In einer Datenbank mit Personen, ist eine Person 
		+ ein **Beispiel $x_i$** aus dem Datensatz
		+ **das erste feature $x_i^{(1)}$** könnte Größe in cm sein
		+ **das erste feature $x_i^{(2)}$** könnte Gewicht in kg sein
		+ **das erste feature $x_i^{(3)}$** könnte Geschlecht sein
	+ Bedeutet wenn **$x_i^{2}$** Gewicht in kg beinhaltet in einem Beispiel $x_i$, dann hat auch **$x_{i+1}^{2}$** Gewicht in kg als 2. feature stehen. 
+ **Das Label $y_i$** zum Beispiel $x_i$
	+ Element einer Klasse (Kategorie zu der das Beispiel gehört), einer Zahl
	+ Beispiel: E-Mails
		+ Problem: Spam-Detection
		+ Dann haben wir 2 Klassen (Spam & Not-Spam)
+ **Ziel**
	+ Algorithmus von supervised learning soll ein Modell anhand eines Datensatzes erstellen, dass einen Merkmals Vektor $x$ als Eingabe bekommt. $x$ könnte ein Sample (Person) sein und es wird die Wahrscheinlichkeit ausgeben ob Person an Krebs erkrankt ist.

[^1]: Ein Vektor der für jede Dimension ein Wert hat. Der Wert beschreibt das Beispiel auf irgendeine Art und Weise. Der Wert wird feature genannt. 
