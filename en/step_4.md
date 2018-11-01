## Coding your world

Let's allow the `player` sprite to walk through doors into other rooms.

Your project contains backdrops for additional rooms:

![screenshot](images/world-backdrops.png)

--- task ---
Create a new 'for all sprites' variable called `room`{:class="blockdata"} to keep track of which room the `player` sprite is in.

[[[generic-scratch-add-variable]]]

![screenshot](images/world-room.png)
--- /task ---

--- task ---
When the `player` sprite touches the orange door in the first room, the next backdrop should be displayed, and the `player` sprite should move back to the left side of the stage. Add this code inside the `player` sprite's `forever`{:class="blockcontrol"} loop:

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
	if < touching color [#BABABA]? > then
	move (-4) steps
	end
+	if < touching color [#F2A24A] > then
	switch backdrop to [next backdrop v]
	go to x: (-200) y: (0)
	change [room v] by (1)
	end
end
```
--- /task ---

--- task ---
At the start of the game the room, character position and backdrop need to be reset.

Add code to the **start** of your `player` sprite code above the `forever`{:class="blockcontrol"} loop, to make sure that everything is reset when the flag is clicked:

--- hints --- --- hint ---
When the game starts, you want the `room`{:class="blockdata"} to be set to `1`{:class="blockdata"}.
You also want the `backdrop`{:class="blocklooks"} to be set to `room1`{:class="blocklooks"} and the position of the character to be set to `x: -200 y: 0`{:class="blockmotion"}
--- /hint --- --- hint ---
Here are the extra blocks you need

![player](images/player.png)

```blocks
go to x: (-200) y: (0)

set [room v] to (1)

switch backdrop to [room1 v]
```
--- /hint --- --- hint ---
Here's what your finished script should look like.

![player](images/player.png)

```blocks
when flag clicked
+set [room v] to (1)
+go to x: (-200) y: (0)
+switch backdrop to [room1 v]
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
	if < touching color [#BABABA]? > then
	move (-4) steps
	end
	if < touching color [#F2A24A] > then
	switch backdrop to [next backdrop v]
	go to x: (-200) y: (0)
	change [room v] by (1)
end
end
```
--- /hint --- --- /hints ---

--- /task ---

--- task ---
Click the flag and move your `player` sprite over the orange door. Does your sprite move to the next screen? Does the `room`{:class="blockdata"} variable change to `2`?

![screenshot](images/world-room-test.png)
--- /task ---


