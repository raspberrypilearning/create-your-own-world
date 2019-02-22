## Wyzwanie: rozwiń swój świat

Możesz teraz kontynuować tworzenie własnego świata! Oto kilka pomysłów:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Dodaj dźwięk i muzykę do swojej gry
+ Add more people, enemies, and signs
+ Dodaj czerwone i żółte drzwi i specjalne klucze, aby je otworzyć
+ Dodaj więcej pokoi do swojego projektu
+ Dodaj inne przydatne przedmioty do swojej gry
    
    + Użyj monet, aby uzyskać informacje od innych postaci:

![screenshot](images/world-bribe.png)

+ You could even add doors in the north and south walls of room 1, so that the player can move between rooms in all four directions. For example, your game can have nine rooms in a 3×3 grid. You can then add `3` to the room number to move down one level.

![zrzut ekranu](images/north-south-rooms.png) ![zrzut ekranu](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```