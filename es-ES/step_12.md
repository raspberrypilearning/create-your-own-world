## Desafío: Amplía tu mundo

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

+ Incluso podrías añadir puertas en las paredes norte y sur de la habitación 1, de modo que el jugador pueda moverse entre habitaciones en las cuatro direcciones. For example, your game can have nine rooms in a 3×3 grid. Entonces podrías sumar `3` al número de habitación para moverte al nivel inferior.

![captura de pantalla](images/north-south-rooms.png) ![screenshot](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```