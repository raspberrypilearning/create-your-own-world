## Сплошные стены

\--- task \---

Test your `player` sprite again. Do you see that it can walk through the light grey walls.

![screenshot](images/world-walls.png)

\--- /task \---

\--- task \---

To fix this, you need to make the `player` sprite move back if it touches a light grey wall. Here's the code you need to add inside your `forever`{:class="block3control"} block below the direction blocks:

![player](images/player.png)

```blocks3
когда щёлкнут по зелёному флагу
повторять всегда 
  если <клавиша (стрелка вверх v) нажата? >, то 
    повернуться в направлении (0)
    идти (4) шагов
  end
  если <клавиша (стрелка влево v) нажата? >, то 
    повернуться в направлении (-90)
    идти (4) шагов
  end
  если <клавиша (стрелка вниз v) нажата? >, то 
    повернуться в направлении (-180)
    идти (4) шагов
  end
  если <клавиша [стрелка вправо v] нажата? >, то 
    повернуться в направлении (90)
    идти (4) шагов
  end
  + если < касается цвета [#BABABA]? >, то 
  +   идти (-4) шагов
  + end
end
```

\--- /task \---

\--- task \---

Try to make the `player` sprite move through a wall. If your new code works, this shouldn't be possible.

![screenshot](images/world-walls-test.png)

\--- /task \---