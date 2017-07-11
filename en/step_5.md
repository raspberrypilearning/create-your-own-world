## Coding your world

Let's allow the player to walk through doors into other rooms!



+ Your project contains backdrops for additional rooms:

	![screenshot](images/world-backdrops.png)

+ You'll need a new 'for all sprites' variable called `room`{:class="blockdata"}, to keep track of what room the player is in. 

	![screenshot](images/world-room.png)

+ When the player touches the orange door in the first room, the next backdrop should be displayed, and the player should move back to the left side of the stage. Here's the code you'll need - it should go inside the player's `forever`{:class="blockcontrol"} loop:

	```blocks
		if < touching color [#F2A24A] > then
			switch backdrop to [next backdrop v]
			go to x: (-200) y: (0)
			change [room v] by (1)
		end
	```

+ Add this code to the _start_ of your player code (before the `forever`{:class="blockcontrol"} loop) to make sure that everything is reset when the flag is clicked:

	```blocks
		set [room v] to (1)
		go to x: (-200) y: (0)
		switch backdrop to [room1 v]
	```

+ Click the flag and move your player over the orange door. Does your player move to the next screen? Does the `room`{:class="blockdata"} variable change to 2?

	![screenshot](images/world-room-test.png)

