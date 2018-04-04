## Schilder

Lass uns Schilder zu deiner Welt hinzufügen, um eine Wegweisung für deinen Spieler auf seiner Reise zu bereiten.

+ Dein Projekt beinhaltet ein Willkommens- Schild Sprite:

	![screenshot](images/world-sign.png)

+ Dieses Schild ist nur in Zimmer 1 sichtbar, lass uns jetzt noch weiteren Code zum Schild hinzufügen, um zu gewährleisten, dass dies passiert:

	```blocks
		Wenn die grüne Flagge angeklickt
		wiederhole fortlaufend
   			falls <(room) = [1]> dann
      			zeige dich
   			sonst
      			verstecke dich
   			Ende
		Ende
	```

+ Teste dein Schild, indem du zwischen den Zimmern hin- und hergehst. Dein Schild sollte nur in Zimmer 1 sichtbar sein.

	![screenshot](images/world-sign-test.png)

+ Ein Schild nützt aber nicht viel, wenn nichts darauf steht! Lass uns weiteren Code (in einem separaten Block) hinzufügen, um eine Meldung anzuzeigen, wenn das Schild den Spieler berührt:

	```blocks
		Wenn die grüne Flagge angeklickt
		wiederhole fortlaufend
   			falls <wird [player v] berührt?> dann
      			sage [Willkommen! Kannst du den Schatz finden?]
   			sonst
      			sage []
   			Ende
		Ende
	```
+ Teste dein Schild und du solltest eine Meldung sehen können, wenn der Spieler es berührt.

	![screenshot](images/world-sign-test2.png)

--- challenge ---

## Aufgabe: Schatz gefunden!
Klicke mit der rechten Maustaste auf das Schatzkisten-Sprite und wähle 'show' (zeigen). 

Kannst du es veranlassen, dass das Schatzkisten-Sprite nur in Zimmer 3 erscheint und dann 'Well done!' (Gut gemacht!) sagen, wenn der Spieler die Kiste berührt?


![screenshot](images/world-treasure.png)

--- /challenge ---