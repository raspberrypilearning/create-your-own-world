## Solid walls

+ Test out your player again, and you'll see they have the ability to walk through the light grey walls.

![screenshot](images/world-walls.png)

+ To fix this, you need to move the player, but then move them back if they're touching a light grey wall. Here's the code you'll need to add:

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

Notice the new `if`{:class="blockcontrol"} block.

+ Test this new code by moving below the wall - you shouldn't be able to move up into it.

![screenshot](images/world-walls-test.png)

+ Do the same for the left arrow, moving back if the player is touching a wall. This is how your player code should look so far:

![screenshot](images/world-wall-code.png)

--- challenge ---
+ Add code to your player sprite so that you can’t walk through walls in any direction. Use the code you already have to help you.

--- hints ---
--- hint ---
To stop the player moving through a wall, you need to move them back by 2 in the opposite direction to the one they were moving in.
--- /hint ---
--- hint ---
Here are the blocks you will need to prevent the player from moving down and right through walls

![Solid walls hint](images/hint-move-back.png)
--- /hint ---
--- hint ---
Add this code inside the `if`{:class="blockcontrol"} `key down arrow pressed`{:class="blocksensing"}:

```blocks
if < touching color [#BABABA]? > then
	change y by (2)
end
```

Add this code inside the `if`{:class="blockcontrol"} `key right arrow pressed`{:class="blocksensing"}:

```blocks
if < touching color [#BABABA]? > then
	change x by (-2)
end
```

--- /hint ---
--- /hints ---

--- /challenge ---
