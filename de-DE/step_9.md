## Herausforderung: Einen Gegner hinzufügen

If you want, you can also add patrolling enemies to your game. If the `player` sprite touches an enemy, the game ends.

+ Your game already contains an `enemy` sprite. Füge der Figur von deinem `Gegner` Code hinzu, so dass er nur in Zimmer 2 erscheint.

+ Add code to move the `enemy` sprite and to end the game if the `enemy` sprite touches the `player` sprite. Das geht einfacher mit zwei getrennten Code-Blöcken. So könnte der Code für deinen `Gegner` aussehen:

```blocks3
when flag clicked
forever
if <(room :: variables)=[2]> then
show
else
hide

when flag clicked
forever
if <touching (player v)?> then
stop [all v]

when flag clicked
go to x: (170) y:(0)
forever
repeat (130)
change x by (-1)
end
repeat (130)
change x by (1)
```

+ Test out your new code to make sure that: 
    + The `enemy` sprite only visible in room 2
    + The `enemy` sprite patrols the room
    + The game ends if the `player` sprite touches the `enemy` sprite

Kannst du einen anderen `Gegner` in das Zimmer 3 setzen, der durch den Spalt in der Mauer auf und ab patrouilliert?

![screenshot](images/world-enemy2.png)