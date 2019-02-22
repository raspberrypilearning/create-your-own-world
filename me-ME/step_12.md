## Izazov: proširi svoj svijet

Sada možeš da nastaviš da kreiraš sopstveni svijet! Evo nekoliko ideja:

+ Add more coins to your game in different rooms. Can you let some coins be guarded by patrolling enemies?
+ Change your game's backdrops
+ Dodaj u svoju igru zvukove i muziku
+ Add more people, enemies, and signs
+ Dodaj crvena i žuta vrata, kao i posebne ključeve za njihovo otvaranje
+ Dodaj još soba u svoj svijet
+ Dodaj druge korisne stvari u svoju igru
    
    + Upotrijebi novčiće da dobiješ informacije od drugih osoba:

![screenshot](images/world-bribe.png)

+ Možeš čak da dodaš vrata na sjeverni i južni zid sobe 1, kako bi igrač mogao da se kreće između soba u sva četiri pravca. For example, your game can have nine rooms in a 3×3 grid. Zatim, za spuštanje na niži nivo, možeš broj sobe uvećati za `3`.

![screenshot](images/north-south-rooms.png) ![screenshot](images/number-grid.png)

```blocks3
if <touching color [ ]?> then
switch backdrop to ((costume [number v]) + (3))
go to x:(0) y:(200)
change [room v] by (3)
```