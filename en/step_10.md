## Collecting coins

As your player moves through the world, they can collect coins.

+ Add a new variable valled `coins`{:class="blockdata"} to your project.

+ Right-click on the 'coin' sprite and choose 'show'.

![screenshot](images/world-coins.png)

+ Add code to your coin, so that it only appears in room 1.

+ Add code to your coin sprite, to add 1 to your `coins`{:class="blockdata"} once they've been picked up:

	```blocks
		when flag clicked
		wait until <touching [player v]?>
		change [coins v] by (1)
		stop [other scripts in sprite v]
		hide
	```

	The code `stop other scripts in sprite`{:class="blockcontrol"} is needed so that the coin stops being displayed in room 1 once it's been collected.

+ You'll also need to add code to set your `coins`{:class="blockdata"} variable to 0 at the start of your game.

+ Test your project - collecting your coins should change your score to 1.

--- challenge ---
### Challenge: More coins
Can you add more coins to your game? They can be in different rooms, and some coins could even be guarded by patrolling enemies.

--- /challenge ---
