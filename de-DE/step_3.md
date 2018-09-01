## Die Figur vom `Spieler` bewegen

Beginnen wir mit der Programmierung einer `Spieler`-Figur die sich in deiner Welt umher bewegen kann.

+ Wenn du Scratch online verwendest, öffne das Scratch-Projekt 'Erschaffe deine eigene Welt' hier: <http://jumpto.cc/world-go>{:target="_blank"}. Wenn Du Scratch offline verwendest, kannst du das Projekt [hier](http://jumpto.cc/world-get){:target="_blank"} herunterladen und es dann mit dem offline Editor öffnen. 

![screenshot](images/world-starter.png)

Die Person, die das Spiel spielt, bewegt die Figur des `Spielers` mit den Pfeiltasten herum. Wenn die Person den Pfeil nach oben drückt, musst du dem `Spieler` sagen, dass er mit einer Bewegung nach oben reagieren soll, so dass er sich in die richtige Richtung bewegt.

+ Füge diesen Code der Figur des `Spielers` hinzu:

```blocks
    Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
  falls &ltTaste [Pfeil nach oben v] gedrückt?&gt dann 
    setze Richtung auf (0)
    gehe (4) er-Schritt
  end
end  
```

+ Teste die Figur deines `Spielers`, indem du auf die Flagge klickst und dann den Pfeil nach oben gedrückt hältst. Bewegt sich dein `Spieler` nach oben?
    
    ![screenshot](images/world-up.png)

+ Um den `Spieler` nach links zu bewegen, musst du einen weiteren `falls`{:class="blockcontrol"}-Block mit ähnlichem Code hinzufügen:

```blocks
    Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
  falls &ltTaste [Pfeil nach oben v] gedrückt? > dann 
    setze Richtung auf (0)
    gehe (4) er-Schritt
  end
  falls <Taste [Pfeil nach links v] gedrückt? > dann 
    setze Richtung auf (-90)
    gehe (4) er-Schritt
  end
end
```

+ Füge deinem `Spieler` mehr code hinzu, damit er sich auch nach unten und nach rechts bewegen kann. Verwende den bereits geschriebenen Code als Hilfe.

\--- hints \--- \--- hint \--- Um nach oben zu gehen, hast du den `Spieler` in Richtung `0` Grad dirigiert. Was hättest du machen müssen, um die Figur nach unten zu bewegen?

Um nach links zu gehen, hast du die Figur nach ` -90` Grad ausgerichtet. Was hättest du machen müssen, um die Figur nach rechts zu bewegen? \--- /hint \--- \--- hint \--- Du musst diese beiden Blöcke ändern:

```blocks
<Taste [ v] gedrückt?>
```

```blocks
setze Richtung auf ()
```

Kopiere den Code den du verwendet hast um nach oben zu gehen, aber ändere diese beiden Blöcke damit sich die Figur des `Spielers` nach unten bewegt. Mache das Gleiche um nach rechts zu gehen. \--- /hint \--- \--- hint \--- Here is how your code should look:

![Moving down and right](images/finished-move-down-right.png) \--- /hint \--- \--- /hints \---