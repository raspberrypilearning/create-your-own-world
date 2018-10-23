## Doors and keys

What if some of the doors in your world are locked, and the player must find the key to progress?

--- task ---
Switch to the `key` sprite. Right-click on it and choose **show** so that it appears on the stage.
--- /task ---

--- task ---
Edit the `key` sprite's costume so that it is blue.
--- /task ---

--- task ---
Switch your Stage backdrop to room 3, and place the `key` sprite somewhere difficult to reach!

 ![screenshot](images/world-key.png)

--- /task ---

--- task ---
Add code to the `key` sprite to make sure that it is only visible in room 3.
--- /task ---

--- task ---
Create a new list variable called `inventory`{:class="blockdata"}. This will be where you store all of the items your `player` sprite collects.

[[[generic-scratch-make-list]]]
--- /task ---

--- task ---
The code for collecting the key is very similar to the code for collecting coins. The difference is that you add the key to your inventory.

![key](images/key.png)

```blocks
when flag clicked
wait until <touching [player v]?>
add [blue key] to [inventory v]
hide
stop [other scripts in sprite v]
```
--- /task ---

--- task ---
Test out your `key` sprite to see if you can collect it and add it to your inventory. Remember to add code to your Stage to empty your inventory at the start of the game.

```blocks
delete (all v) of [inventory v]
```

--- /task ---

--- task ---
Now let's add the locked door. Right-click on the `door-blue` sprite and select **show**, then position the sprite across the gap in the two walls.

![screenshot](images/world-door.png)
--- /task ---

--- task ---
Add code to the `door-blue` sprite so that it is only visible in room 3.
--- /task ---

--- task ---
The `door-blue` sprite should hide to allow your `player` sprite to pass once you have the blue key in your inventory.

![door](images/door.png)

```blocks
when flag clicked
wait until <[inventory v] contains [blue key]>
stop [other scripts in sprite v]
hide
```
--- /task ---

--- task ---
Test out your project, and see if you can collect the blue key to open the door!
--- /task ---
