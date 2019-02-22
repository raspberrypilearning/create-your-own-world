## Herausforderung: Erweitere deine Welt

Du kannst jetzt mit dem Bau deiner eigenen Welt weitermachen! Hier sind ein paar Vorschläge:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Füge deinem Spiel Töne und Musik hinzu
+ Add more people, enemies, and signs
+ Füge rote und gelbe Türen - und spezielle Schlüssel - hinzu, um sie zu öffnen
+ Füge deiner Welt mehr Zimmer hinzu
+ Füge dem Spiel weitere nützliche Gegenstände hinzu
    
    + Verwende Münzen, um Informationen von anderen Personen zu erhalten:

![Screenshot](images/world-bribe.png)

+ Du kannst sogar Türen in den nördlichen und südlichen Wänden von Zimmer 1 hinzufügen, so dass sich der Spieler in allen vier Richtungen zwischen den Zimmern bewegen kann. For example, your game can have nine rooms in a 3×3 grid. Du kannst dann `3` zu der Zimmernummer addieren, um eine Ebene tiefer zu kommen.

![screenshot](images/north-south-rooms.png) ![Screenshot](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```