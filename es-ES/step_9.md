## Desafío: añadir un enemigo

If you want, you can also add patrolling enemies to your game. If the `player` sprite touches an enemy, the game ends.

+ Your game already contains an `enemy` sprite. Añade código al objeto `enemigo` de manera que solamente aparezca en la habitación 2.

+ Add code to move the `enemy` sprite and to end the game if the `enemy` sprite touches the `player` sprite. Es más fácil hacer esto en bloques de código separados. El código de tu objeto `enemigo` debería quedar así:

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

¿Puedes crear otro objeto `enemigo` en la habitación 3 que patrulle arriba y abajo a través del hueco en la pared?

![captura de pantalla](images/world-enemy2.png)