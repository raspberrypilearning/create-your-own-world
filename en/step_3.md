## Solid walls

--- task ---
Test out your `player` sprite again, and you'll probably notice that they have the ability to walk through the light grey walls.

![screenshot](images/world-walls.png)
--- /task ---

--- task ---
To fix this, you should move the `player` sprite back if they're touching a light grey wall. Here's the code you'll need to add inside your `forever`{:class="blockcontrol"} block below the direction blocks:

![player](images/player.png)

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
		if <key [down arrow v] pressed? > then
		point in direction (-180)
		move (4) steps
	end
		if <key [right arrow v] pressed? > then
		point in direction (90)
		move (4) steps
	end
+	if < touching color [#BABABA]? > then
	move (-4) steps
	end
end
```
--- /task ---

--- task ---
Test this new code: move the `player` sprite below the wall, and then see whether you can move them up into it. If your code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)
--- /task ---
