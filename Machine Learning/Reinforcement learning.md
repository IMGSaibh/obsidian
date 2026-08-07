***
+ Reinforcement learning ist ein Teilgebiet des maschinellen Lernens, bei dem die **Maschine in einer Umgebung „lebt“ und in der Lage ist, den Zustand dieser Umgebung als Vektor von Merkmalen wahrzunehmen**
+ Maschine kann in jedem Zustand Aktionen ausführen. 
+ Verschiedene Aktionen bringen unterschiedliche Belohnungen 
	+ Belohnungen können die Maschine auch in einen anderen Zustand der Umgebung versetzen. 
+ **Eine Strategie ist eine Funktion f (ähnlich wie das Modell beim überwachten Lernen),** die den **feature vector $x_i$** eines Zustands als Eingabe nimmt und eine optimale Aktion ausgibt, die in diesem Zustand ausgeführt werden soll. **Die Aktion ist optimal, wenn sie die erwartete durchschnittliche Belohnung maximiert.**
+ **Das Ziel**
	+ Algorithmus für verstärktes Lernen soll eine Strategie erlernen.
