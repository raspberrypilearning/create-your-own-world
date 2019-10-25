## Herausforderung: Einen Gegner hinzufügen

Wenn Du möchtest, kannst Du deinem Spiel auch patrouillierende Feinde hinzufügen. Wenn der `Spieler` einen Feind berührt, endet das Spiel.

+ Dein Spiel enthält bereits eine `Feind`-Figur. Füge der Figur von deinem `Gegner` Code hinzu, so dass er nur in Zimmer 2 erscheint.

+ Füge Code hinzu, um den `Feind` zu bewegen und das Spiel zu beenden, wenn der `Feind` die `Spieler`-Figur berührt. Das geht einfacher mit zwei getrennten Code-Blöcken. So könnte der Code für deinen `Gegner` aussehen:

```blocks3
Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
falls <(Raum :: variables) = [2]> , dann 
zeige dich
sonst 
verstecke dich

Wenn die grüne Flagge angeklickt
wiederhole fortlaufend 
falls <wird (Spieler v) berührt?> , dann 
stoppe [alles v]

Wenn die grüne Flagge angeklickt
gehe zu x: (170) y: (0)
wiederhole fortlaufend 
wiederhole (130) mal 
ändere x um (-1)
Ende
wiederhole (130) mal 
ändere x um (1)
```

+ Teste deinen neuen Coed und kontrolliere ob: 
    + Die `Feind`-Figur nur in Raum 2 sichtbar ist
    + Die `Feind`-Figur durch den Raum patrouilliert
    + Das Spiel endet, wenn die `Spieler`-Figur die `Feind`-Figur berührt

Kannst du einen anderen `Gegner` in das Zimmer 3 setzen, der durch den Spalt in der Mauer auf und ab patrouilliert?

![screenshot](images/world-enemy2.png)