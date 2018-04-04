## Münzen sammeln

+ Füge eine neue Variable namens `coins`{:class="blockdata"} (Münzen) zu deinem Projekt hinzu.

+ Klicke mit der rechten Maustaste auf das 'coin' (Münzen) Sprite und wähle 'show' (zeigen). 

![screenshot](images/world-coins.png)

+ Füge den Code zu deiner Münze hinzu, sodass sie nur in Zimmer 1 erscheint.

+ Füge Code zu deinem Münzen-Sprite hinzu, um 1 zu deinen `coins`{:class="blockdata"} (Münzen) hinzuzufügen, nachdem eine Münze eingesammelt wurde:

	```blocks
		Wenn die grüne Flagge angeklickt
		warte bis <wird [player v] berührt?>
		ändere [coins v] um (1)
		stoppe [andere Skripte der Figur v]
		verstecke dich
	```

	Der Code `stop other scripts in Sprite`{:class="blockcontrol"} (andere Scripts in Sprite stoppen) wird benötigt, damit die Münze nicht länger in Zimmer 1 angezeigt wird, nachdem sie eingesammelt worden ist.

+ Du musst auch Code hinzufügen, um deine `coins`{:class="blockdata"} (Münzen) Variable bei Spielbeginn auf 0 einzustellen.

+ Teste dein Projekt: Das Sammeln deiner Münzen sollte deine Punktzahl zu 1 ändern.

--- challenge ---

## Aufgabe: Weitere Münzen
Kannst du noch mehr Münzen zu deinem Spiel hinzufügen? Sie können in einem anderen Zimmer platziert werden und manche Münzen könnten sogar von den patroullierenden Feinden bewacht werden.

--- /challenge ---