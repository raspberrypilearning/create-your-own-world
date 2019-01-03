## Collect coins

Your `player` sprite should have be able to collect coins as it moves through the world.

--- task ---
Add a new variable valled `coins`{:class="block3variables"} to your project.
--- /task ---

--- task ---
Right-click on the `coin` sprite and choose **show**.

![screenshot](images/coin.png)
--- /task ---

--- task ---
Add code to your `coin` sprite so that it only appears in room 1.
![screenshot](images/coin.png)
![blocks_1546523567_1711764](images/blocks_1546523567_1711764.png)
--- /task ---


--- task ---

Add code to your `coin` sprite so that the sprite `hides`{:class="block3looks"} and `1`{:class="block3variables"} is added to the `coins`{:class="block3variables"} variable once the `player` sprite touches the `coin` sprite to 'pick it up'.

![coin](images/coin.png)

![blocks_1546523569_7267542](images/blocks_1546523569_7267542.png)

The code `stop other scripts in sprite`{:class="block3control"} is needed so that the `coin` sprite stops being displayed in room 1 once it's been collected.

--- /task ---

--- task ---
Now add code to the Stage to set your `coins`{:class="block3variables"} variable to `0`{:class="block3variables"} at the start of the game.

![stage](images/stage.png)
![blocks_1546523571_379865](images/blocks_1546523571_379865.png)
--- /task ---

--- task ---
Test your game. Collecting a coin should change your `coins` score to `1`{:class="block3variables"}.
--- /task ---

