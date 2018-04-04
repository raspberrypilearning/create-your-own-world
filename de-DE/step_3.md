## Programmiere deine Welt

Lass uns jetzt ermöglichen, dass der Spieler durch die Türen in ein anderes Zimmer gelangen kann!

+ Dein Projekt enthält bereits den Hintergrund für weitere Zimmer:

	![screenshot](images/world-backdrops.png)

+ Du brauchst eine neue 'for all sprites' (für alle Sprites) Variable namens `room`{:class="blockdata"} (Zimmer), um mitverfolgen zu können, in welchem Zimmer sich der Spieler gerade aufhält. 

	![screenshot](images/world-room.png)

+ Wenn der Spieler die orange-farbene Tür im ersten Zimmer berührt, sollte der nächste Hintergrund angezeigt werden und der Spieler sollte sich zurück zur linken Seite des Stadiums bewegen. Hier ist der Code, den du hierfür brauchst: Er sollte innerhalb der `forever`{:class="blockcontrol"} (für immer) Schleife des Spielers eingefügt werden:

	```blocks
		falls <wird Farbe [#F2A24A] berührt?> dann
   			wechsle zu Bühnenbild [nächstes Bühnenbild v]
   			gehe zu x:(-200) y:(0)
   			ändere [room v] um (1)
		Ende
	```

+ Füge diesen Code zum _Start_ deines Spieler-Codes hinzu, (vor der `forever`{:class="blockcontrol"} (für immer) Schleife), um zu gewährleisten, dass alles wieder auf Null gestellt wird, wenn die Flagge angeklickt wird:

	```blocks
		setze [room v] auf (1)
		gehe zu x:(-200) y:(0)
		wechsle zu Bühnenbild [room1 v]
	```

+ Klicke die Flagge und bewege deinen Spieler über die orange-farbene Tür. Geht dein Spieler zum nächsten Bildschirm hinüber? Ändert sich die `room`{:class="blockdata"} Zimmer-Variable zu 2?

	![screenshot](images/world-room-test.png)

--- challenge ---
	
	## Aufgabe: Ins vorherige Zimmer gehen 
Kannst du deinen Spieler ins vorherige Zimmer bewegen, wenn er eine gelbe Tür berührt? Denke daran, dass dieser Code _sehr_ ähnlich sein wird wie der Code, den du bereits hinzugefügt hast, um ins nächste Zimmer zu gelangen.

--- /challenge ---