## Uitdaging: vergroot je wereld

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

+ Je zou zelfs deuren kunnen toevoegen aan de noord- en zuidwanden van kamer 1, zodat de speler in alle vier de richtingen door kamers kan lopen. For example, your game can have nine rooms in a 3×3 grid. Je kunt dan `3` optellen bij het kamernummer om naar een ​​niveau lager te gaan.

![screenshot](images/north-south-rooms.png) ![screenshot](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```