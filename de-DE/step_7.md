## Türen und Schlüssel 

+ Bearbeite das Kostüm des Schlüssel-Sprites, damit es blau ist. Klicke mit der rechten Maustaste auf das Schlüssel-Sprite und wähle 'show' (zeigen), damit es im Stadium erscheint. Schalte dein Stadium zu Hintergrund 3 und platziere den Schlüssel irgendwo hin, wo er schwierig zu erreichen ist!

 	![screenshot](images/world-key.png)

+ Achte darauf, dass dein Schlüssel nur in Zimmer 3 sichtbar ist.

+ Erstelle eine neue Listenvariable namens `inventory`{:class="blockdata"} (Inventar). Dies wird der Ort sein, an dem du all die Gegenstände, die dein Spieler einsammelt, aufbewahrst, bzw. speicherst.

+ Der Code zum Einsammeln des Schlüssels ist sehr ähnlich wie der Code zum Einsammeln der Münzen. Der Unterschied ist, dass du den Schlüssel zu deinem Inventar hinzufügst.

	```blocks
		Wenn die grüne Flagge angeklickt
		warte bis <wird [player v] berührt?>
		füge [blue key] zu [inventory v] hinzu
		stoppe [andere Skripte der Figur v]
		verstecke dich
	```

+ Teste deinen Schlüssel, um zu sehen, ob du ihn einsammeln kannst und ob du ihn zu deinem Inventar hinzufügen kannst. Denke daran, den Code zu deinem Stadium hinzuzufügen und dein Inventar bei Spielbeginn zu leeren.

	```Blöcke
		(lösche (alles v) aus [inventory v]
	```

+ Platziere dein blaues Tür-Sprite quer über der Spalte in den beiden Wänden.

	![screenshot](images/world-door.png)

+ Füge Code zu deiner Tür hinzu, damit sie nur in Zimmer 3 sichtbar ist.

+ Du wirst auch deine blaue Tür verstecken müssen, damit dein Spieler daran vorbei gehen kann, nachdem du den blauen Schlüssel in deinem Inventar hast.

	```blocks
		Wenn die grüne Flagge angeklickt
		warte bis <[inventory v] enthält [blue key]>
		stoppe [andere Skripte der Figur v]
		verstecke dich
	```

+ Teste dein Projekt und schau, ob du den blauen Schlüssel einsammeln kannst, um die Tür zu öffnen!

--- challenge ---

## Aufgabe: Erstelle deine eigene Welt 
Du kannst jetzt fortfahren, deine eigene Welt zu erstellen. Hier sind ein paar Vorschläge:

+ Ändere dein Spielumfeld und deine Spielgrafik;
+ Füge Sound und Musik zu deinem Spiel hinzu;
+ Füge weitere Leute, sowie Feinde, Schilder und Münzen hinzu;
+ Füge rote und gelbe Türen hinzu, die ihre eigenen Schlüssel zum Öffnen benötigen;
+ Füge weitere Zimmer zu deiner Welt hinzu;
+ Füge andere, nützliche Gegenstände zu deinem Spiel hinzu;

+ Benutze Münzen, um Informationen von anderen Leuten zu erhalten;

	![screenshot](images/world-bribe.png)

+ Du könntest auch Türen im Norden und Süden hinzufügen, damit der Spieler in allen 4 Richtungen zwischen den Zimmern hin- und hergehen kann. Zum Beispiel: Wenn du 9 Zimmer hättest, könntest du sie als ein 3 x 3 Raster betrachten. Du kannst dann die Nummer 3 zur Zimmerzahl hinzufügen, um dich 1 Stufe herunter zu bewegen.

	![screenshot](images/world-north-south.png)

--- /challenge ---
