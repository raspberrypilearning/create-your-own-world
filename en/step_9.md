## People

Let's add other people to your world that your player can interact with.



+ Add this code to the person sprite, so that the person talks to your player. This code is very similar to the code you added to your sign:

	```blocks
		when flag clicked
		go to x: (0) y: (-150)
		forever
			if < touching [player v]? > then
				say [Did you know that you can go through orange and yellow doors?]
			else
				say []
			end
		end
	```

+ You could also allow your person to move, by using these two blocks:

	```blocks
		move (1) steps
		if on edge, bounce
	```

	Your person will act differently, depending on whether you place this code inside the `forever`{:class="blockcontrol"} loop or the `if`{:class="blockcontrol"} block. Try both and see which you prefer.

	![screenshot](images/world-person-test.png)

+ Have you noticed that your person flips upside-down. To stop this, click the sprite's information icon (`i`), and click the dot to fix to rotation style.

	![screenshot](images/world-person-rotate.png)

