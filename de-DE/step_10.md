## Münzen sammeln

Deine `Spieler` Figur sollte in der Lage sein, Münzen zu sammeln, während sie sich durch die Welt bewegt.

\--- task \--- Fügen deinem Projekt eine neue Variable hinzu und nenne sie `Münzen`{:class="block3variables"}. \--- /task \---

\--- task \--- Wähle die `Münze`-Figur aus und klicke auf **zeige dich**.

![Screenshot](images/coin.png) \--- /task \---

\--- task \--- Füge Code zu deiner `Münzen`-Figur hinzu, sodass sie nur in Raum 1 erscheint. ![Screenshot](images/coin.png)

```blocks3
Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
  falls <(Raum :: variables) = [1]> , dann 
    zeige dich
  sonst 
    verstecke dich
  end
end
```

\--- /task \---

\--- task \---

Füge Code zu deiner `Münze`-Figur hinzu, sodass sie ` sich versteckt`{:class="block3looks"} und `1`{:class="block3variables"} zu der `Münzen`{:class="block3variables"} Variablen hinzugefügt wird, sobald die `Spieler`-Figur die `Münzen`-Figur berührt, um sie aufzuheben.

![Münze](images/coin.png)

```blocks3
Wenn die grüne Flagge angeklickt
warte bis <wird (Spieler v) berührt?>
ändere [Münzen v] um (1)
verstecke dich
stoppe [andere Skripte der Figur v]
```

Der Code `stoppe andere Skripte der Figur`{:class="block3control"}) wird benötigt, damit das `Münze`-Objekt nicht mehr in Raum 1 angezeigt wird, sobald das Objekt eingesammelt wurde.

\--- /task \---

\--- task \--- Füge nun Code zur Bühne hinzu, um deine `Münzen`{:class="block3variables"} Variable, zu Beginn des Spiels, auf `0`{:class= "block3variables"} zu setzen.

![Bühne](images/stage.png)

```blocks3
Wenn die grüne Flagge angeklickt
setze [Münzen v] auf [0]
```

\--- /task \---

\--- task \--- Teste dein Spiel. Das Sammeln einer Münze sollte deine `Münzen` auf `1`{:class="block3variables"} ändern. \--- /task \---