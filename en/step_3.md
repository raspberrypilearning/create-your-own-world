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
			change y by (2)
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
				change y by (2)
			end
			if <key [left arrow v] pressed? > then
				change x by (-2)
			end
		end
	```

--- challenge ---
+ Can you add more code to your player, so that they can move up, down, left and right. Use the code you already have to help you!

--- hints ---
--- hint ---

--- /hint ---
--- /hints ---

--- /challenge ---
