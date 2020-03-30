## Сплошные стены

\--- task \---

Cнова протестируй свой спрайт `игрок`. Как ты видишь, он может проходить сквозь светло-серые стены.

![снимок экрана](images/world-walls.png)

\--- /task \---

\--- task \---

Чтобы это исправить, тебе необходимо сделать так, чтобы спрайт `игрок` двигался в обратном направлении, если он коснется светло-серой стены. Вот код, который тебе нужно добавить внутри блока `повторять всегда`{:class="block3control"} после блока отвечающего за направления:

![игрок](images/player.png)

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
+   if < touching color [#BABABA]? > then
    move (-4) steps
    end
end
```

\--- /task \---

\--- task \---

Попробуй, может ли спрайт `игрок` пройти сквозь стену. Если твой новый код работает, это не должно быть возможно.

![снимок экрана](images/world-walls-test.png)

\--- /task \---