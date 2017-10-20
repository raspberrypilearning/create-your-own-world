## Solid walls

+ Test out your player again, and you'll see they have the ability to walk through the light grey walls.

![screenshot](images/world-walls.png)

+ To fix this, you need to move the player, but then move them back if they're touching a light grey wall. Here's the code you'll need to add inside your `forever`{:class="blockcontrol"} block, below the direction blocks:

```blocks
	if < touching color [#BABABA]? > then
		move (-4) steps
	end
```

+ Test this new code by moving below the wall - you shouldn't be able to move up into it.

![screenshot](images/world-walls-test.png)
