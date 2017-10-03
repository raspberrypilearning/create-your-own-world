## Signs

Let's add signs to your world, to guide the player on their journey.

+ Your project includes a welcome sign sprite:

![screenshot](images/world-sign.png)

+ The sign should only be visible in room 1, so add some code to the sign sprite to make sure that this happens:

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

+ Test your sign by moving between rooms. Your sign should only be visible in room 1.

	![screenshot](images/world-sign-test.png)

+ A sign isn't much good if it doesn't say anything! Add some more code to display a message if the sign is touching the player:

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

+ Test out your sign, and you should see a message when the player touches it.

![screenshot](images/world-sign-test2.png)
