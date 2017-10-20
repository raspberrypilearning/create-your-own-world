## People

Let's add other people to your world that your player can interact with.

+ Switch to the person sprite

![Person sprite](images/person-sprite.png)

+ Add some code to the person sprite, so that the person talks to the player. This code is very similar to the code you added to your sign:

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

+ You could also allow your person to move, by adding these two blocks in the `else`{:class="blockcontrol"} section of your code:

```blocks
move (1) steps
if on edge, bounce
```

Your person will move, but will stop to talk to the player.

![screenshot](images/world-person-test.png)

+ Have you noticed that your person flips upside-down. To stop this, click the sprite's information icon (`i`), and click the dot to fix the rotation style.

![screenshot](images/world-person-rotate.png)


--- challenge ---
### Improve the person
Can you add code to your new person, so that they only appear in room 1? Make sure you test out your new code.

--- /challenge ---
