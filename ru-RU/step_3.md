## Сплошные стены

--- task ---

Cнова протестируй свой спрайт `игрок`. Do you see that it can walk through the light grey walls?

![снимок экрана](images/world-walls.png)

--- /task ---

--- task ---

Чтобы это исправить, тебе необходимо сделать так, чтобы спрайт `игрок` двигался в обратном направлении, если он коснется светло-серой стены. Вот код, который тебе нужно добавить внутри блока `повторять всегда`{:class="block3control"} после блока отвечающего за направления:

![игрок](images/player.png)

```blocks3
when flag clicked
forever
	if <key (стрелка вверх v) pressed? > then
		point in direction (0)
		move (4) steps
	end
	if <key (стрелка влево v) pressed? > then
		point in direction (-90)
		move (4) steps
	end
		if <key (стрелка вниз v) pressed? > then
		point in direction (-180)
		move (4) steps
	end
		if <key (стрелка вправо v) pressed? > then
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

Попробуй, может ли спрайт `игрок` пройти сквозь стену. Если твой новый код работает, это не должно быть возможно.

![снимок экрана](images/world-walls-test.png)

--- /task ---