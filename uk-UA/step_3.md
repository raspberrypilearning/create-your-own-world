## Тверді стіни

\--- task \---

Протестуй свій спрайт `гравець` знову. Ти бачиш, що він може проходити крізь світло-сірі стіни?

![знімок екрана](images/world-walls.png)

\--- /task \---

\--- task \---

Щоб це виправити, тобі треба змусити спрайт `гравець` рухатися назад, як тільки він доторкнеться до сірої стіни. Ось код, який тобі треба буде додати всередині свого блоку `завжди`{:class="block3control"} під блоками для напряму:

![гравець](images/player.png)

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
        point in direction (180)
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

Спробуй пройти спрайтом `гравець` крізь стіну. Якщо твій новий код працює правильно, це має бути неможливо.

![знімок екрана](images/world-walls-test.png)

\--- /task \---