## Moving the player

Let's start by creating a player that can move around your world.

+ Open the 'Create Your Own World' Scratch project online at [http://jumpto.cc/world-go](http://jumpto.cc/world-go){:target="_blank"} or download from [http://jumpto.cc/world-get](http://jumpto.cc/world-get){:target="_blank"} and then open if you are using the offline editor.  

![screenshot](images/world-starter.png)

The player will use the arrow keys to move around. When the player presses the up arrow, you want the player sprite to move up, by changing its y coordinate.

+ Add this code to the `player` sprite:

```blocks
	when flag clicked
	forever
		if <key [up arrow v] pressed? > then
			point in direction (0)
            move (4) steps
		end
	end
```

+ Test out your player by clicking the flag and then holding down the up arrow. Does your player move up?

	![screenshot](images/world-up.png)

+ To move the player to the left, you need to add another `if`{:class="blockcontrol"} block to your player, which changes the x coordinate:

```blocks
	when flag clicked
	forever
		if <key [up arrow v] pressed? > then
			point in direction (0)
            move (4) steps
		end
        if <key [left arrow v] pressed? > then
			point in direction (-90)
            move (4) steps
		end
	end
```

+ Add more code to your player sprite so that they can move down and right as well. Use the code you already have to help you.

--- hints ---
--- hint ---
To move up, you point in the direction 0 degrees. What would you have to do to move the player down?

To move left, you point in the direction -90 degrees. What would you have to do to move the player right?
--- /hint ---
--- hint ---
You will need to change these two blocks:
```blocks
<key [ v] pressed>
```
```blocks
point in direction ()
```

Duplicate the code you have used to go up, but change these two blocks to make the character move down. Do the same for right.
--- /hint ---
--- hint ---
Here is how your code should look:

![Moving down and right](images/finished-move-down-right.png)
--- /hint ---
--- /hints ---
