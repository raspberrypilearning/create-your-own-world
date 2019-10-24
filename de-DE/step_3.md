## Massive Wände

--- task --- Teste deine `Spieler`-Figur nochmal. Siehst du, dass sie durch die hellgrauen Wände gehen kann.

![Screenshot](images/world-walls.png) --- /task ---

--- task --- Um dies zu beheben, musst du die `Spieler`-Figur zurück gehen lassen, wenn es eine hellgraue Wand berührt. Hier ist der Code, den du innerhalb des `wiederholen fortlaufend`{:class="block3control"} -Blocks unter den Richtungs-Blöcken hinzufügen musst:

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
    falls <Taste (Pfeil nach unten v) gedrückt?> , dann 
      setze Richtung auf (-180) Grad
      gehe (4) er Schritt
    falls <Taste [Pfeil nach rechts v] gedrückt?> , dann 
      setze Richtung auf (90) Grad
      gehe (4) er Schritt
+   falls <wird Farbe [#BABABA] berührt?> , dann 
    gehe (-4) er Schritt
end
```

--- /task ---

--- task ---

Versuche, die `Spieler`-Figur durch eine Wand zu bewegen. Wenn dein neuer Code richtig funktioniert, sollte das nicht möglich sein.

![Screenshot](images/world-walls-test.png) --- /task ---