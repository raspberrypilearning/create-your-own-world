## Signs

Now add signs to your world to guide players on their journey.

Your project includes a `welcome sign` sprite:

![screenshot](images/world-sign.png)

--- task ---
The `welcome sign` sprite should only be visible in room 1, so add some code to the sprite to make sure that this happens:

--- hints --- --- hint ---
`When the flag is clicked`{:class="block3events"}, in a `forever`{:class="block3control"} loop, check `if`{:class="block3control"} the `room is 1`{:class="block3variables"} and in that case `show`{:class="block3looks"} `welcome sign` sprite, `else`{:class="block3control"} `hide`{:class="block3looks"} the sprite.
--- /hint --- --- hint ---
Here are the blocks you need:

![sign](images/sign.png)

![blocks_1546523592_9668815](images/blocks_1546523592_9668815.png)
--- /hint --- --- hint ---
Here is the complete code:

![sign](images/sign.png)

![blocks_1546523594_634697](images/blocks_1546523594_634697.png)
--- /hint --- --- /hints ---


--- /task ---

--- task ---
Test the code for your `welcome sign` sprite by moving between rooms. The sign should only be visible in room 1.

![screenshot](images/world-sign-test.png)
--- /task ---

--- task ---
A sign isn't much good if it doesn't say anything! Add some more code to display a message if the `welcome sign` sprite is touching the `player` sprite:

![sign](images/sign.png)

![blocks_1546523596_2368014](images/blocks_1546523596_2368014.png)
--- /task ---

--- task ---
Test your `welcome sign` sprite again. You should now see a message when the `player` sprite touches the `welcome sign` sprite.

![screenshot](images/world-sign-test2.png)
--- /task ---
