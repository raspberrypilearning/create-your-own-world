## Programmiere deinen Spieler

Lass uns damit beginnen, einen Spieler zu erstellen, der sich rund um deine Welt bewegen kann.

+ Öffne das 'Create Your Own World' (Erstelle deine eigene Welt) Scratch Projekt online unter <a href="http://jumpto.cc/world-go" target="_blank">jumpto.cc/world-go</a> oder lade es von <a href="http://jumpto.cc/world-get" target="_blank">jumpto.cc/world-get</a> herunter und öffne es dann, wenn du den offline Editor benutzt.

	![screenshot](images/world-starter.png)

+ Lass uns die Pfeiltasten benutzen, um den Spieler rund ums Spielfeld zu bewegen. Wenn der Spieler die Pfeil-hoch-Taste drückt, dann willst du, dass der Spieler nach oben geht, indem wir dessen y-Koordinaten ändern. Füge diesen Code zum `player` (Spieler) Sprite hinzu:

	```blocks
		Wenn die grüne Flagge angeklickt
		wiederhole fortlaufend
   			falls <Taste [Pfeil nach oben v] gedrückt?> dann
      			ändere y um (2)
   			Ende
		Ende
	```

+ Teste deinen Spieler, indem du auf die Flagge klickst und dann die Pfeil-hoch-Taste gedrückt hältst. Bewegt sich dein Spieler nach oben?

	![screenshot](images/world-up.png)

+ Um den Spieler nach links zu bewegen, musst du einen weiteren `if` {.blockcontrol} (wenn) Block zu deinem Spieler hinzufügen, welcher dann die x-Koordinaten ändert:

	```blocks
		Wenn die grüne Flagge angeklickt
		wiederhole fortlaufend
  			falls <Taste [Pfeil nach oben v] gedrückt?> dann
      			ändere y um (2)
   			Ende
   			falls <Taste [Pfeil nach links v] gedrückt?> dann
      			ändere x um (-2)
   			Ende
		Ende
	```

--- challenge ---
	
## Aufgabe: Sich in alle vier Richtungen bewegen
Kannst du noch mehr Code zu deinem Spieler hinzufügen, damit er sich nach oben, nach unten, nach links oder nach rechts bewegen kann. Benutze den Code, den du bereits hast, um dir hierbei zu helfen!

+ Teste deinen Spieler erneut und du wirst sehen, dass er die Fähigkeit hat, durch die hellgrauen Wände durchzugehen.

	![screenshot](images/world-walls.png)

+ Um dieses Problem zu beheben, musst du den Spieler bewegen, aber ihn dann zurück bewegen, wenn er eine hellgraue Wand berührt. Hier ist der Code den du brauchst:

	```blocks
		Wenn die grüne Flagge angeklickt
		wiederhole fortlaufend
   			falls <Taste [Pfeil nach oben v] gedrückt?> dann
      			ändere y um (2)
      			falls <wird Farbe [#BABABA] berührt?> dann
         			ändere y um (-2)
      			Ende
   			Ende
		Ende
	```

	Hast du gemerkt, dass der neue `if`{:class="blockcontrol"} (wenn) `touching color`{:class="blocksensing"} (Farbe berührt) Block sich _innerhalb_ des `if`{:class="blockcontrol"} (wenn) `key [up arrow]`{:class="blocksensing"} (Schlüssel [Pfeil hoch]) Blocks befindet?

+ Teste diesen neuen Code, indem du unter die Wand gehst (du solltest nicht in der Lage sein, in die Wand hoch zu gehen).

	![screenshot](images/world-walls-test.png)

+ Lass uns das Gleiche für die linke Pfeiltaste tun, gehe zurück, wenn der Spieler eine Wand berührt. Hier ist, wie der Code für deinen Spieler bislang aussehen sollte:

	![screenshot](images/world-wall-code.png)

--- /challenge ---

--- challenge ---
	
## Aufgabe: Repariere die Bewegung deines Spielers 
Füge Code zu deinem Spieler hinzu, damit er nicht in jede Richtung durch die Wand laufen kann. Benutze den Code, den du bereits hast, um dir hierbei zu helfen!

--- /challenge ---