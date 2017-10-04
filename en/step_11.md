## Doors and keys

What if some of the doors in your world are locked, and the player must find the key to progress?

+ Switch to the key sprite. Right-click on it and choose 'show' so that it appears on the stage.

+ Edit the key sprite's costume so that it is blue.

+  Switch your stage backdrop to room 3, and place the key somewhere difficult to reach!

 ![screenshot](images/world-key.png)

+ Add some code to the key sprite to make sure that the key is only visible in room 3.

+ Create a new list variable called `inventory`{:class="blockdata"}. This will be where you store all of the items your player collects.

[[[generic-scratch-make-list]]]

+ The code for collecting the key is very similar to the code for collecting coins. The difference is that you add the key to your inventory.

```blocks
	when flag clicked
	wait until <touching [player v]?>
	add [blue key] to [inventory v]
	stop [other scripts in sprite v]
	hide
```

+ Test out your key, to see if you can collect it, and add it to your inventory. Remember to add code to your stage to empty your inventory at the start.

```blocks
	delete (all v) of [inventory v]
```

+ Now let's add the locked door. Right click on the blue door sprite and select 'show', then position the sprite across the gap in the two walls.

![screenshot](images/world-door.png)

+ Add code to the blue door, so that it is only visible in room 3.

+ The blue door should hide to allow your player to pass once you have the blue key in your inventory.

```blocks
	when flag clicked
	wait until <[inventory v] contains [blue key]>
	stop [other scripts in sprite v]
	hide
```

+ Test out your project, and see if you can collect the blue key to open the door!
