## Uitdaging: voeg een vijand toe

If you want, you can also add patrolling enemies to your game. If the `player` sprite touches an enemy, the game ends.

+ Your game already contains an `enemy` sprite. Voeg code toe aan de sprite `vijand` zodat die alleen in kamer 2 verschijnt.

+ Add code to move the `enemy` sprite and to end the game if the `enemy` sprite touches the `player` sprite. Het is makkelijker om dat in verschillende blokken code te doen. Zo zou sprite `vijand` eruit kunnen zien:

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

Kun je nog een sprite `vijand` maken in kamer 3 die op en neer beweegt door het gat in de muur?

![screenshot](images/world-enemy2.png)