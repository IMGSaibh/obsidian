***
## Ich habe gerade verloren, aber es gab definitiv einen Weg
+ [ ] Jede Partie ist beim Start garantiert lösbar – aber nicht jeder Zug führt noch zu einer Lösung
	+ [ ] **Foundation → Tableau nicht erlauben.** Eine Karte auf die Foundation zu legen ist dann eine echte Entscheidung. Legst du sie zu früh ab, kannst du dir möglicherweise einen notwendigen Tableau-Zug verbauen.
	+ [ ] **Tableau-Züge bleiben endgültig**, außer der Spieler verwendet Undo.
	+ [ ] **Stock/Waste-Regeln ebenfalls so wählen, dass Entscheidungen relevant sind.** Unbegrenztes Durchklicken des Stocks nimmt einiges an Schwierigkeit heraus.
	+ [ ] Der Deal selbst wird vor Spielbeginn von einem Solver geprüft: Es existiert mindestens **eine vollständige Lösung**.
	+ [ ] Garantieren, dass ein Spiel **ohne Undo lösbar** ist
+ [ ] Man kann danach erneut denselben Deal starten und versuchen herauszufinden, **welche Entscheidung falsch war**.
## Undo als Schwierigkeitsgrad
+ [ ] Schwierigkeit
	+ [ ] Entspannt -> unbegrenzt undo
	+ [ ] Normal -> 10 undo
	+ [ ] Schwer -> 3 undo
	+ [ ] Expert -> 0 undo
+ [ ] **Undo als Ressource sichtbar zu machen**
## Nice to have
+ [ ] Dieser Deal war lösbar. Du warst 84 % des Lösungswegs entfernt
+ [ ] Deine Partie wurde mit Zug 37 unlösbar.