--- challenge ---
## Challenge: Moving in all four directions
Can you add more code to your player, so that they can move up, down, left and right. Use the code you already have to help you!



+ Test out your player again, and you'll see they have the ability to walk through the light grey walls.

	![screenshot](images/world-walls.png)

+ To fix this, you need to move the player, but then move them back if they're touching a light grey wall. Here's the code you'll need:

	```blocks
		when flag clicked
		forever
			if <key [up arrow v] pressed? > then
				change y by (2)
				if < touching color [#BABABA]? > then
					change y by (-2)
				end
			end
		end
	```

	Notice that the new `if`{.blockcontrol}`touching color`{.blocksensing} block is _inside_ the `if`{.blockcontrol}`key [up arrow]`{.blocksensing} block.

+ Test this new code by moving below the wall - you shouldn't be able to move up into it.

	![screenshot](images/world-walls-test.png)

+ Let's do the same for the left arrow, moving back if the player is touching a wall. This is how your player code should look so far:

	![screenshot](images/world-wall-code.png)


--- /challenge ---