## Programmiere deinen Spieler

Beginne mit der Erstellung einer `Spieler`-Figur, die sich in deiner Welt umher bewegen kann.

--- task ---

Öffne das "Erstelle deine eigene Welt" Scratch Starter Projekt.

**Online:** öffne das Basisprojekt auf [scratch.mit.edu/projects/339073366](https://scratch.mit.edu/projects/339073366){:target="_blank"}.

Wenn du bereits einen Scratch-Account besitzt, kannst du dir durch Klick auf **Remix** eine Kopie anlegen.

**Offline:** Wenn du offline arbeiten möchtest, kannst du dir die benötigte Datei unter [rpf.io/p/de-DE/create-your-own-world-go](http://rpf.io/p/de-DE/create-your-own-world-go){:target="_blank"} herunterladen und diese dann mit dem Offline-Editor bearbeiten. Wenn du Scratch herunterladen und auf deinem Rechner installieren möchtest, dann findest du die Datei unter diesem Link: [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

![screenshot](images/world-starter.png)

--- /task ---

Durch Drücken der Pfeiltasten sollte sich die `Spieler`-Figur herum bewegen. Wenn der Aufwärtspfeil gedrückt wird, sollte sich die `Spieler`-Figur als Reaktion auf der Bühne nach oben bewegen.

--- task ---

Füge diesen Code zur `Spieler`-Figur hinzu:

![Spieler](images/player.png)

```blocks3
Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
  falls <Taste (Pfeil nach oben v) gedrückt?> , dann 
     setze Richtung auf (0) Grad
     gehe (4) er Schritt
```

--- /task ---

--- task ---

Klicke auf die Flagge und halte den Aufwärtspfeil gedrückt. Bewegt sich dein `Spieler` nach oben?

![screenshot](images/world-up.png)

--- /task ---

--- task ---

Um die `Spieler`-Figur nach links zu bewegen, musst du einen weiteren `falls`{:class="block3control"}-Block mit ähnlichem Code hinzufügen:

![player](images/player.png)

```blocks3
Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
    falls <Taste (Pfeil nach oben v) gedrückt?> , dann 
        setze Richtung auf (0) Grad
        gehe (4) er Schritt
+   falls <Taste (Pfeil nach links v) gedrückt?> , dann 
        setze Richtung auf (-90) Grad
        gehe (4) er Schritt
```

--- /task ---

--- task ---

Füge deinem `Spieler` weiteren Code hinzu, damit er sich auch nach unten und nach rechts bewegen kann. Verwende den bereits geschriebenen Code als Hilfe.

--- hints ---


--- hint ---

Um nach oben zu gehen, musst du den `Spieler` in Richtung `0` Grad zeigen lassen. Was musst du machen, um die Figur nach unten zu bewegen?

Um nach links zu gehen, muss die Figur in Richtung ` -90` Grad zeigen lassen. Was musst du machen, um die Figur nach rechts zu bewegen?

--- /hint ---

--- hint ---

Du musst diese beiden Blöcke ändern:

![player](images/player.png)

```blocks3
<Taste ( v) gedrückt?>

setze Richtung auf () Grad
```

Dupliziere den Code, der die `Spieler`-Figur nach oben bewegt und ändere diese beiden Blöcke, damit sich die Figur nach unten bewegt. Dupliziere den Code erneut und ändere ihn, damit sich die Figur nach rechts bewegt.

--- /hint --- --- hint --- Dein Code sollte so aussehen:

![player](images/player.png)

```blocks3
Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
    falls <Taste (Pfeil nach oben v) gedrückt?> , dann 
            setze Richtung auf (0) Grad
            gehe (4) er Schritt
    falls <Taste (Pfeil nach links v) gedrückt?> , dann 
            setze Richtung auf (-90) Grad
            gehe (4) er Schritt
+    falls <Taste (Pfeil nach unten v) gedrückt?> , dann 
            setze Richtung auf (180) Grad
            gehe (4) er Schritt
     end 
+    falls <Taste [Pfeil nach rechts v] gedrückt?> , dann 
            setze Richtung auf (90) Grad
            gehe (4) er Schritt
```

--- /hint ------ /hints ---

--- /task ---