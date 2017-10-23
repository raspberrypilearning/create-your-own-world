## Collecting coins

As your `player` sprite moves through the world, they can collect coins.

+ Add a new variable valled `coins`{:class="blockdata"} to your project.

+ Right-click on the `coins` sprite and choose **show**.

![screenshot](images/world-coins.png)

+ Add code to your `coins` sprite so that it only appears in room 1.

+ Add code to your `coins` sprite so that `1` is added to `coins`{:class="blockdata"} once the coin has been picked up:

	```blocks
		when flag clicked
		wait until <touching [player v]?>
		change [coins v] by (1)
		stop [other scripts in sprite v]
		hide
	```

	The code `stop other scripts in sprite`{:class="blockcontrol"} is needed so that the `coins` sprite stops being displayed in room 1 once it's been collected.

+ You'll also need to add code to set your `coins`{:class="blockdata"} variable to `0` at the start of your game.

+ Test your project — collecting a coin should change your score to `1`.

--- challenge ---
### Challenge: more coins
Can you add more coins to your game? They can be in different rooms, and some coins could even be guarded by patrolling enemies!

--- /challenge ---
