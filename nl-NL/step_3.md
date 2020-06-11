## Stevige muren

--- task --- Test je `speler` sprite opnieuw. Zie je dat het door de lichtgrijze muren kan lopen.

![screenshot](images/world-walls.png) --- /task ---

--- task --- Om dit te verhelpen, moet je de `speler` sprite zo maken dat deze terug beweegt als het een lichtgrijze muur raakt. Dit is de code die je moet toevoegen in je `herhaal`{:class="block3control"}-blok onder de blokken voor de richting:

![speler](images/player.png)

```blocks3
when flag clicked
forever
	if <key (up arrow v) pressed? > then
		point in direction (0)
		move (4) steps
	end
	if <key (left arrow v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
		if <key (down arrow v) pressed? > then
		point in direction (-180)
		move (4) steps
	end
		if <key (right arrow v) pressed? > then
		point in direction (90)
		move (4) steps
	end
+	if < touching color [#BABABA]? > then
	move (-4) steps
	end
end
```

--- /task ---

--- task ---

Probeer de `speler` sprite door een muur te verplaatsen. Als je nieuwe code werkt, zou dit niet mogelijk moeten zijn.

![screenshot](images/world-walls-test.png) --- /task ---