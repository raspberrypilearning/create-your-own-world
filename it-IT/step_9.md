## Sfida: aggiungi un nemico

If you want, you can also add patrolling enemies to your game. If the `player` sprite touches an enemy, the game ends.

+ Your game already contains an `enemy` sprite. Aggiungi del codice allo sprite `nemico` per far sì che appaia solo nella stanza 2.

+ Add code to move the `enemy` sprite and to end the game if the `enemy` sprite touches the `player` sprite. È più facile farlo in blocchi di codice separati. Ecco come il codice del tuo sprite `nemico` potrebbe apparire:

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

Sapresti creare un altro sprite `nemico` nella stanza 3 che pattugli su e giù attraverso lo spazio nel muro?

![screenshot](images/world-enemy2.png)