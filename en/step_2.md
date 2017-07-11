## Coding your player

Let's start by creating a player that can move around your world.



+ Open the 'Create Your Own World' Scratch project online at <a href="http://jumpto.cc/world-go" target="_blank">jumpto.cc/world-go</a> or download from <a href="http://jumpto.cc/world-get" target="_blank">jumpto.cc/world-get</a> and then open if you are using the offline editor.

	![screenshot](images/world-starter.png)

+ Let's use the arrow keys to move the player around. When the player presses the up arrow, you want the player to move up, by changing its y coordinate. Add this code to the `player` sprite:

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

