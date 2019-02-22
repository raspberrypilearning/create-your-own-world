## Herausforderung: Erweitere deine Welt

You can now continue creating your own world! Here are some ideas:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Add sound and music to your game
+ Add more people, enemies, and signs
+ Add red and yellow doors, and special keys to open them
+ Add more rooms to your world
+ Add other useful items to your game
    
    + Use coins to get information from other people:

![screenshot](images/world-bribe.png)

+ Du kannst sogar Türen in den nördlichen und südlichen Wänden von Zimmer 1 hinzufügen, so dass sich der Spieler in allen vier Richtungen zwischen den Zimmern bewegen kann. For example, your game can have nine rooms in a 3×3 grid. Du kannst dann `3` zu der Zimmernummer addieren, um eine Ebene tiefer zu kommen.

![screenshot](images/north-south-rooms.png) ![screenshot](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```