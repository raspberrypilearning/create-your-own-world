## Moving the `player` sprite

Let's start by creating a `player` sprite that can move around your world.

--- task ---

--- collapse ---
---
title: Starting your project
---

If you're using Scratch online, open the 'Create your own world' Scratch project at [http://rpf.io/p/en/on](http://rpf.io/p/en/on){:target="_blank"}.

If you are using Scratch offline, download the project [http://rpf.io/p/en/off](http://rpf.io/p/en/off){:target="_blank"}, and then open it using the 
offline editor.

--- /collapse ---

![screenshot](images/world-starter.png)

--- /task ---

The person playing the game will use the arrow keys to move the `player` sprite around. When the person presses the up arrow, you need to tell the `player` sprite to move up in response, so that it moves in the right direction.

--- task ---

Add this code to the `player` sprite:

![player](images/player.png)

```blocks
when flag clicked
forever
	if <key [up arrow v] pressed? > then
		point in direction (0)
		move (4) steps
	end
end
```

--- /task ---

--- task ---

Test out your `player` sprite by clicking the flag and then holding down the up arrow. Does your `player` sprite move up?

![screenshot](images/world-up.png)

--- /task ---

--- task ---

To move the `player` sprite to the left, you need to add another `if`{:class="blockcontrol"} block with similar code to it:

--- hints --- --- hint ---
You can use the same code you have above, but this time use the `key left arrow pressed?`{:class="blocksensing"} and set the direction to `-90`{:class="blockmovement"}
--- /hint --- --- hint ---
Here are the new blocks you will need
![player](images/player.png)
```blocks
if < > then
end

move (4) steps

point in direction (-90)

<key [left arrow v] pressed? >

```
--- /hint --- --- hint ---
![player](images/player.png)

```blocks
when flag clicked
forever
	if <key [up arrow v] pressed? > then
		point in direction (0)
		move (4) steps
	end
+	if <key [left arrow v] pressed? > then
		point in direction (-90)
		move (4) steps
	end
end
```

--- /hint --- --- /hints ---
--- /task ---

--- task ---

Add more code to your `player` sprite so that they can move down and right as well. Use the code you already have to help you.

--- hints ---
--- hint ---
To move up, you pointed the `player` sprite into the direction `0` degrees. What would you have to do to move the sprite down?

To move left, you pointed the sprite in the direction `-90` degrees. What would you have to do to move the sprite right?
--- /hint ---
--- hint ---
You will need to change these two blocks:

![player](images/player.png)

```blocks
<key [ v] pressed>

point in direction ()
```

Duplicate the code you have used to go up, but change these two blocks to make the `player` sprite move down. Do the same for moving right.
--- /hint ---
--- hint ---
Here is how your code should look:

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
+		if <key [down arrow v] pressed? > then
		point in direction (-180)
		move (4) steps
	end
+		if <key [right arrow v] pressed? > then
		point in direction (90)
		move (4) steps
	end
end
```
--- /hint ---
--- /hints ---

--- /task ---
