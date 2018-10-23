## Signs

Let's add signs to your world to guide the player on their journey.

--- task ---
Your project includes a `welcome sign` sprite:

![screenshot](images/world-sign.png)
--- /task ---

--- task ---
The `welcome sign` sprite should only be visible in room 1, so add some code to the `welcome sign` sprite to make sure that this happens:

--- hints --- --- hint ---
`When the flag is clicked`{:class="blockevents"} within a `forever`{:class="blockcontrol"} loop `if`{:class="blockcontrol"} the `room is 1`{:class="blockdata"} then the sign sprite should `show`{:class="blocklooks"}, `else`{:class="blockcontrol"} the sprite should `hide`{:class="blocklooks"}
--- /hint --- --- hint ---
Here are the blocks you will need:

![sign](images/sign.png)

```blocks

if < > then
else
end

< (room) = [1] >

hide

show

forever
end

when flag clicked
end
```
--- /hint --- --- hint ---
Here is the complete code.

![sign](images/sign.png)

```blocks
when flag clicked
forever
	if < (room) = [1] > then
		show
	else
		hide
	end
end
```
--- /hint --- --- /hints ---


--- /task ---

--- task ---
Test your `welcome sign` sprite by moving between rooms. Your sign should only be visible in room 1.

![screenshot](images/world-sign-test.png)
--- /task ---

--- task ---
A sign isn't much good if it doesn't say anything! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

![sign](images/sign.png)

```blocks
when flag clicked
forever
	if < (room) = [1] > then
		show
	else
		hide
	end
	if < touching [player v]? > then
		say [Welcome! Can you get to the treasure?]
	else
		say []
	end
end
```
--- /task ---

--- task ---
Test out your `welcome sign` sprite — you should now see a message when the `player` sprite touches it.

![screenshot](images/world-sign-test2.png)
--- /task ---
