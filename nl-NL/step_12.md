## Uitdaging: vergroot je wereld

Je kunt nu doorgaan met het maken van je eigen wereld! Hier zijn wat ideeën:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Voeg geluid en muziek toe aan je spel
+ Add more people, enemies, and signs
+ Voeg rode en gele deuren toe en bijzondere sleutels om ze te openen
+ Voeg meer kamers toe aan je wereld
+ Voeg andere nuttige dingen toe aan je spel
    
    + Gebruik munten om informatie van andere personen te krijgen:

![screenshot](images/world-bribe.png)

+ Je zou zelfs deuren kunnen toevoegen aan de noord- en zuidwanden van kamer 1, zodat de speler in alle vier de richtingen door kamers kan lopen. For example, your game can have nine rooms in a 3×3 grid. Je kunt dan `3` optellen bij het kamernummer om naar een ​​niveau lager te gaan.

![screenshot](images/north-south-rooms.png) ![screenshot](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```