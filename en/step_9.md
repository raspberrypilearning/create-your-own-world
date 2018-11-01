## Challenge: add an enemy

You could also add in patrolling enemies. If the player touches an enemy, the game ends.

+ Add code to the `enemy` sprite so that it only appears in room 2.

+ Add code to move the `enemy` sprite, and to end the game if the `enemy` sprite touches the `player` sprite. It's easier to do this in separate code blocks. Here's how your `enemy` sprite code might look:

```blocks
when flag clicked
forever
if <(room)=[2]> then
show
else
hide

when flag clicked
forever
if <touching [player v]?> then
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

+ Test out your `enemy` sprite to make sure that:
	+ It's only visible in room 2
	+ It patrols the room
	+ The game ends if the `player` sprite touches it


Can you create another `enemy` sprite in room 3 that patrols up and down through the gap in the wall?

![screenshot](images/world-enemy2.png)

